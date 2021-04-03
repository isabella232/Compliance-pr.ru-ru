---
title: Удаление данных Microsoft 365 SharePoint Online
description: Узнайте, как происходит удаление данных в SharePoint Online, например, где хранится удаленный контент и как долго.
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: Normal
search.appverid:
- MET150
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- SPO_Content
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: e89a261e44ef4eb4a1399027b70be88fffb82036
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51497416"
---
# <a name="sharepoint-online-data-deletion-in-microsoft-365"></a><span data-ttu-id="27194-103">Удаление данных SharePoint Online в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="27194-103">SharePoint Online data deletion in Microsoft 365</span></span>

<span data-ttu-id="27194-104">SharePoint Online хранит объекты в качестве абстрактного кода в базах данных приложений.</span><span class="sxs-lookup"><span data-stu-id="27194-104">SharePoint Online stores objects as abstracted code within application databases.</span></span> <span data-ttu-id="27194-105">Когда пользователь загружает файл в SharePoint Online, он разобрано и переведено в код приложения и хранится в нескольких таблицах в нескольких базах данных.</span><span class="sxs-lookup"><span data-stu-id="27194-105">When a user uploads a file to SharePoint Online, that file is disassembled and translated into application code and stored in multiple tables across multiple databases.</span></span> <span data-ttu-id="27194-106">В SharePoint Online все загружаемое клиентом содержимое разбивается на куски, шифруется (возможно, с несколькими клавишами AES 256-bit) и распространяется через центр обработки данных.</span><span class="sxs-lookup"><span data-stu-id="27194-106">In SharePoint Online, all content that a customer uploads is broken into chunks, encrypted (potentially with multiple AES 256-bit keys), and distributed across the datacenter.</span></span> <span data-ttu-id="27194-107">Подробные сведения о процессе ломки и шифрования см. в материале [Encryption in the Microsoft Cloud.](/microsoft-365/compliance/office-365-encryption-in-the-microsoft-cloud-overview)</span><span class="sxs-lookup"><span data-stu-id="27194-107">For specific details about the chunking and encryption process, see [Encryption in the Microsoft Cloud](/microsoft-365/compliance/office-365-encryption-in-the-microsoft-cloud-overview).</span></span> 

<span data-ttu-id="27194-108">В SharePoint Online элементы сохраняются в течение 93 дней с того времени, как вы удалите их из исходного расположения.</span><span class="sxs-lookup"><span data-stu-id="27194-108">In SharePoint Online, items are retained for 93 days from the time you delete them from their original location.</span></span> <span data-ttu-id="27194-109">Они остаются на сайте Recycle Bin все время, если кто-то удаляет их оттуда или опустошает это корзины.</span><span class="sxs-lookup"><span data-stu-id="27194-109">They stay in the site Recycle Bin the entire time, unless someone deletes them from there or empties that Recycle Bin.</span></span> <span data-ttu-id="27194-110">В этом случае элементы перейдут в корзину корзины веб-сайтов, где они остаются в течение оставшегося 93 дня.</span><span class="sxs-lookup"><span data-stu-id="27194-110">In that case, the items go to the site collection Recycle Bin, where they stay for the remainder of the 93 days.</span></span> <span data-ttu-id="27194-111">Сведения о восстановлении удаленных элементов см. в раздел Восстановление элементов в корзине сайта [SharePoint](https://support.office.com/article/6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online
) и восстановление удаленных элементов из корзины коллекции [сайтов.](https://support.office.com/article/5fa924ee-16d7-487b-9a0a-021b9062d14b)</span><span class="sxs-lookup"><span data-stu-id="27194-111">For info about restoring deleted items, see [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online
) and [Restore deleted items from the site collection recycle bin](https://support.office.com/article/5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span> <span data-ttu-id="27194-112">Время хранения корзины в SharePoint Online не настраивается.</span><span class="sxs-lookup"><span data-stu-id="27194-112">The Recycle Bin retention time is not configurable in SharePoint Online.</span></span>

<span data-ttu-id="27194-113">При удалении коллекции сайтов также удаляется иерархия сайтов в коллекции и весь контент в них:</span><span class="sxs-lookup"><span data-stu-id="27194-113">When you delete a site collection, you're also deleting the hierarchy of sites in the collection, and all content within them:</span></span>

- <span data-ttu-id="27194-114">документы и библиотеки документов;</span><span class="sxs-lookup"><span data-stu-id="27194-114">Documents and document libraries</span></span>
- <span data-ttu-id="27194-115">Списки и данные списков</span><span class="sxs-lookup"><span data-stu-id="27194-115">Lists and list data</span></span>
- <span data-ttu-id="27194-116">Параметры конфигурации сайта</span><span class="sxs-lookup"><span data-stu-id="27194-116">Site configuration settings</span></span>
- <span data-ttu-id="27194-117">Сведения о роли и безопасности, связанные с сайтом или его подзаймами</span><span class="sxs-lookup"><span data-stu-id="27194-117">Role and security information that is related to the site or its subsites</span></span>
- <span data-ttu-id="27194-118">Subsites of the top-level website, their contents, and user information</span><span class="sxs-lookup"><span data-stu-id="27194-118">Subsites of the top-level website, their contents, and user information</span></span>

<span data-ttu-id="27194-119">Если вы случайно удалите коллекцию сайтов, она может быть восстановлена глобальным администратором или администратором SharePoint с помощью центра администрирования SharePoint.</span><span class="sxs-lookup"><span data-stu-id="27194-119">If you accidentally delete a site collection, it can be restored by a global or SharePoint admin using the SharePoint admin center.</span></span>

<span data-ttu-id="27194-120">Удаленные коллекции сайтов сохраняются в течение 93 дней.</span><span class="sxs-lookup"><span data-stu-id="27194-120">Deleted site collections are retained for 93 days.</span></span> <span data-ttu-id="27194-121">По истечении 93 дней сайты и все их содержимое с параметрами, в том числе списки, библиотеки, страницы и любые дочерние сайты, удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="27194-121">After 93 days, sites and all their content and settings are permanently deleted, including lists, libraries, pages, and any subsites.</span></span>

<span data-ttu-id="27194-122">Жесткое удаление происходит, когда пользователь очищает удаленные элементы из корзины коллекции сайтов, когда истекает срок хранения и резервного копирования, или когда администратор постоянно удаляет коллекцию сайтов с помощью [cmdlet Remove-SPODeletedSite.](/powershell/module/sharepoint-online/remove-spodeletedsite)</span><span class="sxs-lookup"><span data-stu-id="27194-122">Hard deletion occurs when a user purges deleted items from the site collection Recycle Bin, when the retention and backup periods expire, or when an administrator permanently deletes a site collection using the [Remove-SPODeletedSite cmdlet](/powershell/module/sharepoint-online/remove-spodeletedsite).</span></span> <span data-ttu-id="27194-123">Когда пользователь с трудом удаляет (постоянно удаляет или очищает) контент из SharePoint Online, все ключи шифрования удаленных фрагментов также удаляются.</span><span class="sxs-lookup"><span data-stu-id="27194-123">When a user hard deletes (permanently deletes, or purges) content from SharePoint Online, all encryption keys for the deleted chunks are also deleted.</span></span> <span data-ttu-id="27194-124">Блоки на дисках, на которые ранее хранились удаленные фрагменты, помечены как неиспользимые и доступны для повторного использования.</span><span class="sxs-lookup"><span data-stu-id="27194-124">The blocks on the disks that previously stored the deleted chunks are marked as unused and available for re-use.</span></span>
