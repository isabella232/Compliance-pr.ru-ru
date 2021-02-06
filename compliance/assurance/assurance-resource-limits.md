---
title: Ограничения ресурсов Microsoft 365
description: В этой статье вы найдете сведения об ограничениях ресурсов для различных приложений в Microsoft 365.
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
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: 632a0b78c5c5ba02a59f8863c2e751f009cc968e
ms.sourcegitcommit: 21ed42335efd37774ff5d17d9586d5546147241a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2021
ms.locfileid: "50120758"
---
# <a name="service-resource-limits"></a><span data-ttu-id="dc603-103">Ограничения ресурсов служб</span><span class="sxs-lookup"><span data-stu-id="dc603-103">Service resource limits</span></span>

<span data-ttu-id="dc603-104">Ограничения ресурсов применяются с помощью квот (ограничений) и регулирования.</span><span class="sxs-lookup"><span data-stu-id="dc603-104">Resource limits are enforced using quotas (limits) and throttling.</span></span> <span data-ttu-id="dc603-105">Azure Active Directory (Azure AD) и отдельные службы Microsoft 365 используют обе службы.</span><span class="sxs-lookup"><span data-stu-id="dc603-105">Azure Active Directory (Azure AD) and the individual Microsoft 365 services use both.</span></span> <span data-ttu-id="dc603-106">Ограничения специфичен для служб и со временем изменяются по мере того, как добавляются новые возможности.</span><span class="sxs-lookup"><span data-stu-id="dc603-106">Limits are service-specific and change over time as new capabilities are added.</span></span> <span data-ttu-id="dc603-107">Сведения о текущих ограничениях для различных служб см. в следующих темах:</span><span class="sxs-lookup"><span data-stu-id="dc603-107">For details on the current limits for the various services, see the following topics:</span></span>

- [<span data-ttu-id="dc603-108">Ограничения для служб Azure AD</span><span class="sxs-lookup"><span data-stu-id="dc603-108">Azure AD service limits and restrictions</span></span>](/azure/azure-resource-manager/management/azure-subscription-service-limits)
- [<span data-ttu-id="dc603-109">Ограничения Exchange Online</span><span class="sxs-lookup"><span data-stu-id="dc603-109">Exchange Online Limits</span></span>](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)
- [<span data-ttu-id="dc603-110">Ограничения для программного обеспечения SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="dc603-110">SharePoint Online software boundaries and limits</span></span>](https://support.office.com/article/SharePoint-Online-software-boundaries-and-limits-8F34FF47-B749-408B-ABC0-B605E1F6D498)
- [<span data-ttu-id="dc603-111">Ограничения Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="dc603-111">Skype for Business Limits</span></span>](https://technet.microsoft.com/library/skype-for-business-online-limits.aspx)
- [<span data-ttu-id="dc603-112">Rest API Yammer и ограничения скорости</span><span class="sxs-lookup"><span data-stu-id="dc603-112">Yammer REST API and Rate Limits</span></span>](https://developer.yammer.com/docs/rest-api-rate-limits)
- [<span data-ttu-id="dc603-113">Ограничения на размер файлов в Sway</span><span class="sxs-lookup"><span data-stu-id="dc603-113">File Size Limits in Sway</span></span>](https://support.office.com/article/File-size-limits-in-Sway-4db21bc6-b42b-499f-9272-66e089db109f)

<span data-ttu-id="dc603-114">Помимо этих ограничений, в Azure AD и Microsoft 365 используется несколько механизмов регулирования.</span><span class="sxs-lookup"><span data-stu-id="dc603-114">In addition to these limits, several throttling mechanisms are used throughout Azure AD and Microsoft 365.</span></span> <span data-ttu-id="dc603-115">Регулирование в службе особенно важно, поскольку сетевые ресурсы в центрах обработки данных Майкрософт оптимизированы для широкого круга клиентов, которые используют службы.</span><span class="sxs-lookup"><span data-stu-id="dc603-115">Throttling within the service is especially important, given that network resources in Microsoft's datacenters are optimized for the broad set of customers that use the services.</span></span> <span data-ttu-id="dc603-116">К механизмам регулирования относятся:</span><span class="sxs-lookup"><span data-stu-id="dc603-116">Throttling mechanisms include:</span></span>

- <span data-ttu-id="dc603-117">Регулирование на уровне пользователя в Azure AD и Microsoft 365, ограничивающее количество транзакций или одновредных вызовов (по сценарию или коду), которые может выполнять один пользователь.</span><span class="sxs-lookup"><span data-stu-id="dc603-117">Azure AD and Microsoft 365 feature user-level throttling, which limit the number of transactions or concurrent calls (by script or code) that can be performed by a single user.</span></span>
- <span data-ttu-id="dc603-118">Политика регулирования PowerShell по умолчанию назначена каждому арендатору при создании клиента.</span><span class="sxs-lookup"><span data-stu-id="dc603-118">A default PowerShell throttling policy is assigned to each tenant at tenant creation.</span></span> <span data-ttu-id="dc603-119">Эти параметры влияют на другие элементы, например максимальное количество одновременных сеансов PowerShell, которые может открыть один администратор.</span><span class="sxs-lookup"><span data-stu-id="dc603-119">These settings affect other items, such as the maximum number of simultaneous PowerShell sessions that can be opened by a single administrator.</span></span>
- <span data-ttu-id="dc603-120">Каждый клиент Exchange Online имеет политику веб-служб Exchange (EWS) по умолчанию, настроенную для клиентских операций EWS, и регулирование, которое применяется ко всем клиентам Outlook.</span><span class="sxs-lookup"><span data-stu-id="dc603-120">Each Exchange Online customer has a default Exchange Web Services (EWS) policy that is tuned for EWS client operations, and throttling that applies to all Outlook clients.</span></span>
