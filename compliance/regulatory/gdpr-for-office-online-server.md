---
title: GDPR для Office Online Server и сервера Office Web Apps
description: В этой статье объясняется, как соответствовать требованиям GDPR для Office Online Server и сервера Office Web Apps.
f1.keywords:
- NOCSH
ms.author: mikeplum
author: MikePlumleyMSFT
manager: pamgreen
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: Priority
ms.collection: MS-Compliance
ms.custom:
- seo-marvel-mar2020
titleSuffix: Microsoft GDPR
hideEdit: true
ms.openlocfilehash: 298f0efe74539c8a8bd10330cfeb80894ef9edb1
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53089018"
---
# <a name="gdpr-for-office-web-apps-server-and-office-online-server"></a><span data-ttu-id="406fd-103">GDPR для сервера Office Web Apps и Office Online Server</span><span class="sxs-lookup"><span data-stu-id="406fd-103">GDPR for Office Web Apps Server and Office Online Server</span></span>

<span data-ttu-id="406fd-p101">Данные телеметрии Office Online Server и сервера Office Web Apps хранятся в виде журналов ULS. С помощью приложения [ULS Viewer](https://www.microsoft.com/download/details.aspx?id=44020) вы можете просматривать журналы ULS из локального клиента.</span><span class="sxs-lookup"><span data-stu-id="406fd-p101">Office Online Server and Office Web Apps Server telemetry data is stored in the form of ULS logs. You can use [ULS Viewer](https://www.microsoft.com/download/details.aspx?id=44020) to view ULS logs from your on-premises tenant.</span></span>

<span data-ttu-id="406fd-p102">Каждая строка журнала содержит CorrelationID. Связанные строки журнала имеют одинаковое значение CorrelationID. Каждое значение CorrelationID привязано к одному значению SessionID, а одно значение SessionID может быть связано с несколькими значениями CorrelationID. Каждое значение SessionID может быть связано с одним UserID, но некоторые сеансы могут быть анонимными (с ними не связано значение UserID). Чтобы определить, какие данные связаны с определенным пользователем, можно сопоставить одно значение UserID со значениями SessionID, связанными с этим пользователем, эти значения SessionID — с соответствующими значениями CorrelationID, а эти значения CorrelationID — со всеми журналами для этих сопоставлений. На приведенной ниже схеме показаны отношения между разными идентификаторами.</span><span class="sxs-lookup"><span data-stu-id="406fd-p102">Every log line contains a CorrelationID. Related log lines share the same CorrelationID. Each CorrelationID is tied to a single SessionID, and one SessionID may be related to many CorrelationIDs. Each SessionID may be related to a single UserID, although some sessions can be anonymous and therefore not have an associated UserID. In order to determine what data is associated with a particular user, it is therefore possible to map from a single UserID to the SessionIDs associated with that user, from those SessionIDs to the associated CorrelationIDs, and from those CorrelationIDs to all the logs in those correlations. See the below diagram for the relationship between the different IDs.</span></span>

![Блок-схема, показывающая связь между значениями SessionID и CorrelationId](../media/gdpr-for-office-online-server-image1.jpg)

## <a name="gathering-logs"></a><span data-ttu-id="406fd-113">Сбор журналов</span><span class="sxs-lookup"><span data-stu-id="406fd-113">Gathering Logs</span></span>

<span data-ttu-id="406fd-p103">Чтобы собрать все журналы, связанные, к примеру, с UserID 1, для начала необходимо собрать все сеансы, связанные с UserID 1 (т. е. SessionID 1 и SessionID 2). Затем следует собрать все сопоставления, связанные с SessionID 1 (т. е. CorrelationID 1, 2 и 3) и с SessionID 2 (т. е. CorrelationID 4). Напоследок необходимо собрать все журналы, связанные с каждым из сопоставлений в списке.</span><span class="sxs-lookup"><span data-stu-id="406fd-p103">In order to gather all logs associated with UserID 1, for example, the first step would be to gather all sessions associated with UserID 1 (that is, SessionID 1 and SessionID2). The next step would be to gather all correlations associated with SessionID 1 (that is, CorrelationIDs 1, 2, and 3) and with SessionID 2 (that is, CorrelationID 4). Finally, gather all logs associated with each of the correlations in the list.</span></span>

1. <span data-ttu-id="406fd-117">Запустите средство UlsViewer.</span><span class="sxs-lookup"><span data-stu-id="406fd-117">Launch UlsViewer</span></span>

2. <span data-ttu-id="406fd-118">Откройте журнал ULS, соответствующий нужному временному интервалу. Журналы ULS хранятся в папке %PROGRAMDATA%\\Microsoft\\OfficeWebApps\\Data\\Logs\\ULS.</span><span class="sxs-lookup"><span data-stu-id="406fd-118">Open up the uls log corresponding to the intended timeframe; ULS logs are stored in %PROGRAMDATA%\\Microsoft\\OfficeWebApps\\Data\\Logs\\ULS</span></span>

3. <span data-ttu-id="406fd-119">Измените фильтр.</span><span class="sxs-lookup"><span data-stu-id="406fd-119">Edit | Modify Filter</span></span>

4. <span data-ttu-id="406fd-120">Примените следующий фильтр:</span><span class="sxs-lookup"><span data-stu-id="406fd-120">Apply a filter that is:</span></span>

    - <span data-ttu-id="406fd-121">EventID равно apr3y</span><span class="sxs-lookup"><span data-stu-id="406fd-121">EventID equals apr3y</span></span>

      <span data-ttu-id="406fd-122">или</span><span class="sxs-lookup"><span data-stu-id="406fd-122">Or</span></span>

    - <span data-ttu-id="406fd-123">EventID равно bp2d6</span><span class="sxs-lookup"><span data-stu-id="406fd-123">EventID equals bp2d6</span></span>

5. <span data-ttu-id="406fd-124">Хэшированные значения UserId будут храниться в свойстве Message одного из этих двух событий.</span><span class="sxs-lookup"><span data-stu-id="406fd-124">Hashed UserIds will be in the Message of either one of these two events</span></span>

6. <span data-ttu-id="406fd-125">Для apr3y свойство Message будет содержать значения UserID и PUID.</span><span class="sxs-lookup"><span data-stu-id="406fd-125">For apr3y, the Message will contain a UserID value and a PUID value</span></span>

7. <span data-ttu-id="406fd-p104">Для bp2d6 свойство Message будет содержать довольно много сведений. Поле Value для LoggableUserId — это хэшированный UserID.</span><span class="sxs-lookup"><span data-stu-id="406fd-p104">For bp2d6, the Message will contain quite a bit of information. The LoggableUserId Value field is the hashed UserID.</span></span>

8. <span data-ttu-id="406fd-128">После получения хэшированного значения UserId из одного из этих тегов значение WacSessionId для этой строки в ULSViewer будет содержать WacSessionId, связанный с этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="406fd-128">Once the hashed UserId is obtained from either of these two tags, the WacSessionId value of that row in ULSViewer will contain the WacSessionId associated with that user</span></span>

9. <span data-ttu-id="406fd-129">Соберите все значения WacSessionId, связанные с нужным пользователем.</span><span class="sxs-lookup"><span data-stu-id="406fd-129">Collect all of the WacSessionId values associated with the user in question</span></span>

10. <span data-ttu-id="406fd-130">Примените фильтр — EventId равно "xmnv", Message равно "UserSessionId=\<WacSessionId\>" — к первому значению WacSessionId в списке (замените часть \<WacSessionId\> своим значением WacSessionId)</span><span class="sxs-lookup"><span data-stu-id="406fd-130">Filter for all EventId equals "xmnv", Message equals "UserSessionId=\<WacSessionId\>" for the first WacSessionId in the list (replacing the \<WacSessionId\> part of the filter with your WacSessionId)</span></span>

11. <span data-ttu-id="406fd-131">Соберите все значения свойств Correlation, соответствующие этому WacSessionId.</span><span class="sxs-lookup"><span data-stu-id="406fd-131">Collect all values of Correlation that match that WacSessionId</span></span>

12. <span data-ttu-id="406fd-132">Повторите действия 10–11 со всеми значениями WacSessionId в списке для нужного пользователя.</span><span class="sxs-lookup"><span data-stu-id="406fd-132">Repeat steps 10-11 for all values of WacSessionId in your list for the user in question</span></span>

13. <span data-ttu-id="406fd-133">Примените следующий фильтр: Correlation равно первому значению Correlation в списке.</span><span class="sxs-lookup"><span data-stu-id="406fd-133">Filter for all Correlation equals the first Correlation in your list</span></span>

14. <span data-ttu-id="406fd-134">Соберите все журналы, соответствующие этому значению Correlation.</span><span class="sxs-lookup"><span data-stu-id="406fd-134">Collect all logs matching that Correlation</span></span>

15. <span data-ttu-id="406fd-135">Повторите действия 13–14 со всеми значениями Correlation в списке для нужного пользователя.</span><span class="sxs-lookup"><span data-stu-id="406fd-135">Repeat steps 13-14 for all values of Correlation in your list for the user in question</span></span>

## <a name="types-of-data"></a><span data-ttu-id="406fd-136">Типы данных</span><span class="sxs-lookup"><span data-stu-id="406fd-136">Types of Data</span></span>

<span data-ttu-id="406fd-p105">Журналы Office содержат множество различных типов данных. Журналы ULS могут содержать следующие данные:</span><span class="sxs-lookup"><span data-stu-id="406fd-p105">Office logs contain various different types of data. The following are examples of the data that ULS logs may contain:</span></span>

- <span data-ttu-id="406fd-139">коды ошибок, возникших во время использования продукта;</span><span class="sxs-lookup"><span data-stu-id="406fd-139">Error codes for issues encountered during use of the product</span></span>

- <span data-ttu-id="406fd-140">нажатия кнопок и другие данные об использовании приложений;</span><span class="sxs-lookup"><span data-stu-id="406fd-140">Button clicks and other pieces of data about app usage</span></span>

- <span data-ttu-id="406fd-141">данные о производительности и/или определенных функциях приложения;</span><span class="sxs-lookup"><span data-stu-id="406fd-141">Performance data about the app and/or particular features within the app</span></span>

- <span data-ttu-id="406fd-142">общие сведения о местоположении компьютера пользователя (например, страна или регион, штат и город, полученные из IP-адреса), но не точное географическое положение;</span><span class="sxs-lookup"><span data-stu-id="406fd-142">General location information about where the user's computer is (for example, country / region, state, and city, derived from the IP address), but not precise geo location.</span></span>

- <span data-ttu-id="406fd-143">основные метаданные браузера (например, название и версия) и компьютера (например, тип и версия ОС);</span><span class="sxs-lookup"><span data-stu-id="406fd-143">Basic metadata about the browser, for example, browser name and version, and the computer, for example, OS type and version</span></span>

- <span data-ttu-id="406fd-144">сообщения об ошибках от ведущего приложения документа (например, OneDrive, SharePoint, Exchange);</span><span class="sxs-lookup"><span data-stu-id="406fd-144">Error messages from the document host (for example, OneDrive, SharePoint, Exchange)</span></span>

- <span data-ttu-id="406fd-145">сведения о внутренних процессах приложения, не связанных с какими-либо действиями пользователя.</span><span class="sxs-lookup"><span data-stu-id="406fd-145">Information about processes internal to the app, unrelated to any action the user has taken</span></span>
