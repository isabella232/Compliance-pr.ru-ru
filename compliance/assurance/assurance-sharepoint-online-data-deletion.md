---
title: Microsoft 365 SharePoint Удаление данных в Интернете
description: Узнайте, как удаление данных работает в SharePoint Online, например, где хранится удаленный контент и как долго.
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
search.appverid:
- MET150
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- SPO_Content
- MS-Compliance
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 3545a6e5746553e59603fbf68432ee4705a21f3f
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/23/2021
ms.locfileid: "58481711"
---
# <a name="sharepoint-online-data-deletion-in-microsoft-365"></a>SharePoint Удаление данных в интернете в Microsoft 365

SharePoint Он-лайн хранит объекты как абстрактный код в базах данных приложений. Когда пользователь загружает файл в SharePoint Online, он разобрано и переведено в код приложения и хранится в нескольких таблицах в нескольких базах данных. В SharePoint Online все содержимое, загружаемое клиентом, разбивается на куски, шифруется (возможно, с несколькими ключами AES 256-bit) и распространяется через центр обработки данных. Подробные сведения о процессе ломки и шифрования см. в материале [Encryption in the Microsoft Cloud.](/microsoft-365/compliance/office-365-encryption-in-the-microsoft-cloud-overview) 

В SharePoint Online элементы сохраняются в течение 93 дней со времени удаления их из исходного расположения. Они остаются на сайте Recycle Bin все время, если кто-то удаляет их оттуда или опустошает это корзины. В этом случае элементы перейдут в корзину корзины веб-сайтов, где они остаются в течение оставшегося 93 дня. Сведения о восстановлении удаленных [](https://support.office.com/article/6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online
) элементов см. в статьи Восстановление элементов в корзине SharePoint сайта и восстановление удаленных элементов из корзины коллекции [сайтов.](https://support.office.com/article/5fa924ee-16d7-487b-9a0a-021b9062d14b) Время хранения корзины не настраивается в SharePoint Online.

При удалении коллекции сайтов также удаляется иерархия сайтов в коллекции и весь контент в них:

- документы и библиотеки документов;
- Списки и данные списков
- Параметры конфигурации сайта
- Сведения о роли и безопасности, связанные с сайтом или его подзаймами
- Subsites of the top-level website, their contents, and user information

Если вы случайно удалите коллекцию сайтов, она может быть восстановлена глобальным или администратором SharePoint с помощью центра администрирования SharePoint.

Удаленные коллекции сайтов сохраняются в течение 93 дней. По истечении 93 дней сайты и все их содержимое с параметрами, в том числе списки, библиотеки, страницы и любые дочерние сайты, удаляются без возможности восстановления.

Жесткое удаление происходит, когда пользователь очищает удаленные элементы из корзины коллекции сайтов, когда истекает срок хранения и резервного копирования, или когда администратор постоянно удаляет коллекцию сайтов с помощью [cmdlet Remove-SPODeletedSite.](/powershell/module/sharepoint-online/remove-spodeletedsite) Когда пользователь с трудом удаляет (постоянно удаляет или очищает) содержимое SharePoint Online, все ключи шифрования удаленных фрагментов также удаляются. Блоки на дисках, на которые ранее хранились удаленные фрагменты, помечены как неиспользимые и доступны для повторного использования.
