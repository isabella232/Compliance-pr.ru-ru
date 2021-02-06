---
title: Элементы управления административным доступом в Microsoft 365
description: В этой статье представлен обзор элементов управления административным доступом и категоризации данных в Microsoft 365.
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
f1.keywords:
- NOCSH
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: d3d6cd30fbe682de979d5c04943c57cedc86552f
ms.sourcegitcommit: 21ed42335efd37774ff5d17d9586d5546147241a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2021
ms.locfileid: "50120718"
---
# <a name="administrative-access-controls-in-microsoft-365"></a><span data-ttu-id="d70f8-103">Элементы управления административным доступом в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d70f8-103">Administrative access controls in Microsoft 365</span></span> 

<span data-ttu-id="d70f8-104">Корпорация Майкрософт активно вкладывает средства в системы и элементы управления, автоматизющие большинство операций Microsoft 365, намеренно ограничив доступ к контенту клиентов корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="d70f8-104">Microsoft has invested heavily in systems and controls that automate most Microsoft 365 operations while intentionally limiting access to customer content by Microsoft.</span></span> <span data-ttu-id="d70f8-105">Люди управляют службой, а программное обеспечение управляет службой.</span><span class="sxs-lookup"><span data-stu-id="d70f8-105">Humans govern the service, and software operates the service.</span></span> <span data-ttu-id="d70f8-106">Эта структура позволяет Корпорации Майкрософт управлять Microsoft 365 в масштабе и управлять рисками внутренних угроз для контента клиентов.</span><span class="sxs-lookup"><span data-stu-id="d70f8-106">This structure enables Microsoft to manage Microsoft 365 at scale and manage the risks of internal threats to customer content.</span></span>

<span data-ttu-id="d70f8-107">По умолчанию инженеры Корпорации Майкрософт не имеют постоянных прав администратора и не имеют постоянного доступа к контенту клиентов в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d70f8-107">By default, Microsoft engineers have zero standing administrative privileges and zero standing access to customer content in Microsoft 365.</span></span> <span data-ttu-id="d70f8-108">Инженер майкрософт может иметь ограниченный, проверенный и защищенный доступ к контенту клиента в течение ограниченного времени.</span><span class="sxs-lookup"><span data-stu-id="d70f8-108">A Microsoft engineer can have limited, audited, and secured access to a customer's content for a limited amount of time.</span></span> <span data-ttu-id="d70f8-109">Доступ необходим только при необходимости для операций службы и только при одобрении членом высшего руководства Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="d70f8-109">Access is only when necessary for service operations and only when approved by a member of Microsoft senior management.</span></span> <span data-ttu-id="d70f8-110">Для клиентов с лицензией на доступ к окнам клиентского доступа клиент предоставляет разрешение на доступ к их контенту, который содержится в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d70f8-110">For Customer Lockbox licensed customers, the customer provides access approval to their content hosted on Microsoft 365.</span></span>

<span data-ttu-id="d70f8-111">Корпорация Майкрософт предоставляет веб-службы с использованием нескольких способов доставки в облако:</span><span class="sxs-lookup"><span data-stu-id="d70f8-111">Microsoft provides online services using multiple forms of cloud delivery:</span></span>

- <span data-ttu-id="d70f8-112">**Общедоступные облака:** Включает многоканальный набор версий Microsoft 365, Azure и других служб, которые были в Северной Америке, Южной Америке, Европе, Азии, Австралии и т. д.</span><span class="sxs-lookup"><span data-stu-id="d70f8-112">**Public clouds:** Includes multi-tenant versions of Microsoft 365, Azure, and other services hosted in North America, South America, Europe, Asia, Australia, etc.</span></span>
- <span data-ttu-id="d70f8-113">**Национальные облака:** Включает все независимые и сторонние облака за пределами США (за исключением ранее отмеченных), таких как Microsoft 365 в Китае (под управлением 21Vianet) и Microsoft 365 в Германии (под управлением корпорации Майкрософт, но в модели, в которой немецкий доверятель данных Deutsche Telekom контролирует и отслеживает доступ корпорации Майкрософт к данным клиентов и системам, которые содержат данные клиента).</span><span class="sxs-lookup"><span data-stu-id="d70f8-113">**National clouds:** Includes all sovereign and third party-operated clouds outside of the United States (except ones noted previously), such as Microsoft 365 in China (operated by 21Vianet), and Microsoft 365 in Germany (operated by Microsoft, but under a model in which a German data trustee, Deutsche Telekom, controls and monitors Microsoft's access to customer data and systems that contain customer data).</span></span>
- <span data-ttu-id="d70f8-114">**Облака для государственных органов:** Включает службы Microsoft 365 и Azure, доступные для государственных клиентов США.</span><span class="sxs-lookup"><span data-stu-id="d70f8-114">**Government clouds:** Includes Microsoft 365 and Azure services that are available to United States government customers.</span></span>

<span data-ttu-id="d70f8-115">Для целей этой статьи службы Microsoft 365 включают:</span><span class="sxs-lookup"><span data-stu-id="d70f8-115">For purposes of this article, Microsoft 365 services include:</span></span>

- [<span data-ttu-id="d70f8-116">Exchange Online</span><span class="sxs-lookup"><span data-stu-id="d70f8-116">Exchange Online</span></span>](/Exchange/exchange-online)
- [<span data-ttu-id="d70f8-117">Exchange Online Protection</span><span class="sxs-lookup"><span data-stu-id="d70f8-117">Exchange Online Protection</span></span>](/Office365/SecurityCompliance/eop/exchange-online-protection-overview)
- [<span data-ttu-id="d70f8-118">SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d70f8-118">SharePoint Online</span></span>](/sharepoint/sharepoint-online)
- [<span data-ttu-id="d70f8-119">OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="d70f8-119">OneDrive for Business</span></span>](/OneDrive/onedrive)
- [<span data-ttu-id="d70f8-120">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="d70f8-120">Skype for Business</span></span>](/SkypeForBusiness/skype-for-business-online)
- [<span data-ttu-id="d70f8-121">Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d70f8-121">Microsoft Teams</span></span>](/MicrosoftTeams/Teams-overview)
- [<span data-ttu-id="d70f8-122">Yammer</span><span class="sxs-lookup"><span data-stu-id="d70f8-122">Yammer</span></span>](/yammer/yammer-landing-page)

## <a name="microsoft-365-access-controls"></a><span data-ttu-id="d70f8-123">Элементы управления доступом Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d70f8-123">Microsoft 365 access controls</span></span>

<span data-ttu-id="d70f8-124">В целях контроля доступа майкрософт классифицируют данные Microsoft 365 как данные клиента или другие типы данных.</span><span class="sxs-lookup"><span data-stu-id="d70f8-124">For access control purposes, Microsoft categorizes Microsoft 365 data as customer data or other types of data.</span></span>

### <a name="customer-data"></a><span data-ttu-id="d70f8-125">Данные клиента</span><span class="sxs-lookup"><span data-stu-id="d70f8-125">Customer data</span></span>

<span data-ttu-id="d70f8-126">Данные клиента — это все данные, предоставляемые клиентом или от его имени при использовании служб Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d70f8-126">Customer data is all data provided by or on behalf of a customer when using Microsoft 365 services.</span></span> <span data-ttu-id="d70f8-127">Эти данные — это контент клиента, непосредственно созданный или загруженный пользователями Microsoft 365, в том числе:</span><span class="sxs-lookup"><span data-stu-id="d70f8-127">This data is customer content directly created or uploaded by Microsoft 365 users, including:</span></span>

- <span data-ttu-id="d70f8-128">Сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="d70f8-128">Emails</span></span>
- <span data-ttu-id="d70f8-129">Контент SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d70f8-129">SharePoint Online content</span></span>
- <span data-ttu-id="d70f8-130">Мгновенные сообщения</span><span class="sxs-lookup"><span data-stu-id="d70f8-130">Instant messages</span></span>
- <span data-ttu-id="d70f8-131">Элементы календаря</span><span class="sxs-lookup"><span data-stu-id="d70f8-131">Calendar items</span></span>
- <span data-ttu-id="d70f8-132">Документы</span><span class="sxs-lookup"><span data-stu-id="d70f8-132">Documents</span></span>
- <span data-ttu-id="d70f8-133">Контакты</span><span class="sxs-lookup"><span data-stu-id="d70f8-133">Contacts</span></span>
- <span data-ttu-id="d70f8-134">Личные сведения конечных пользователей (EUII) (данные, уникальные для пользователя или которые можно связать с отдельным пользователем, но не включают контент клиента)</span><span class="sxs-lookup"><span data-stu-id="d70f8-134">End-user identifiable information (EUII) (data that is unique to a user or that is linkable to an individual user but does not include customer content)</span></span>

### <a name="other-types-of-data"></a><span data-ttu-id="d70f8-135">Другие типы данных</span><span class="sxs-lookup"><span data-stu-id="d70f8-135">Other types of data</span></span>

<span data-ttu-id="d70f8-136">К другим типам данных относятся:</span><span class="sxs-lookup"><span data-stu-id="d70f8-136">Other types of data include:</span></span>

- <span data-ttu-id="d70f8-137">**Данные учетной записи:** Включает административные данные (сведения, предоставляемые администраторами при регистрации или покупке услуг), а также платежные данные (сведения об инструментах оплаты, например сведения о кредитных картах).</span><span class="sxs-lookup"><span data-stu-id="d70f8-137">**Account data:** Includes administrative data (information provided by administrators when they sign-up or purchase services), and payment data (information about payment instruments, such as credit card details).</span></span>
- <span data-ttu-id="d70f8-138">**Информация, идентифицируемая в организации:** Включает данные, используемые для идентификации клиента, данные об использовании и не могут быть привязыны к отдельному пользователю или включены в контент клиента.</span><span class="sxs-lookup"><span data-stu-id="d70f8-138">**Organizationally identifiable information:** Includes data used to identify a tenant, usage data, and not linkable to an individual user or included in customer content.</span></span>
- <span data-ttu-id="d70f8-139">**Системные метаданные:** Включает журналы служб, содержащие параметры конфигурации, состояние системы, IP-адреса Майкрософт и технические сведения о подписках и клиентах.</span><span class="sxs-lookup"><span data-stu-id="d70f8-139">**System metadata:** Includes service logs that contain configuration settings, system status, Microsoft IP addresses, and technical information about subscriptions and tenants.</span></span>

<span data-ttu-id="d70f8-140">Корпорация Майкрософт установила механизмы контроля доступа, чтобы ни у одного из них не было неодобренного доступа к данным клиента или данным контроля доступа.</span><span class="sxs-lookup"><span data-stu-id="d70f8-140">Microsoft has established access control mechanisms to ensure that no one has unapproved access to Customer Data or access control data.</span></span> <span data-ttu-id="d70f8-141">Данные управления доступом управляют доступом к другим типам данных или функциям в среде, включая доступ к контенту клиента или EUII, паролям Майкрософт, сертификатам безопасности и другим данным, связанным с проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="d70f8-141">Access control data manages access to other types of data or functions within the environment, including access to customer content or EUII, Microsoft passwords, security certificates, and other authentication-related data.</span></span> <span data-ttu-id="d70f8-142">Механизмы контроля доступа также защититься от неодобренного физического, логического или удаленного доступа к производственной среде Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d70f8-142">Access control mechanisms also guard against unapproved physical, logical, or remote access to the Microsoft 365 production environment.</span></span>

<span data-ttu-id="d70f8-143">Существует три категории элементов управления доступом, используемых корпорацией Майкрософт для работы с Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="d70f8-143">There are three categories of access controls used by Microsoft for operating Microsoft 365:</span></span>

- <span data-ttu-id="d70f8-144">Элементы управления изоляцией</span><span class="sxs-lookup"><span data-stu-id="d70f8-144">Isolation controls</span></span>
- <span data-ttu-id="d70f8-145">Средства контроля персонала</span><span class="sxs-lookup"><span data-stu-id="d70f8-145">Personnel controls</span></span>
- <span data-ttu-id="d70f8-146">Технологические элементы управления</span><span class="sxs-lookup"><span data-stu-id="d70f8-146">Technology controls</span></span>

<span data-ttu-id="d70f8-147">В сочетании эти элементы управления помогают предотвращать и обнаруживать вредоносные действия в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d70f8-147">When combined, these controls help prevent and detect malicious actions in Microsoft 365.</span></span> <span data-ttu-id="d70f8-148">В дополнение к изоляции, персоналу и технологическим средствам контроля, используемым корпорацией Майкрософт, существует четвертая категория средств контроля: эти средства контроля реализованы клиентами.</span><span class="sxs-lookup"><span data-stu-id="d70f8-148">In addition to the isolation, personnel, and technology controls used by Microsoft, there is a fourth category of controls: those controls implemented by customers.</span></span>

<span data-ttu-id="d70f8-149">Microsoft 365 позволяет управлять данными так же, как и в локальной среде.</span><span class="sxs-lookup"><span data-stu-id="d70f8-149">Microsoft 365 allows you to manage data the same way data is managed in on-premises environments.</span></span> <span data-ttu-id="d70f8-150">Человек, который подписывает организацию на Microsoft 365, автоматически становится глобальным администратором.</span><span class="sxs-lookup"><span data-stu-id="d70f8-150">The person who signs up an organization for Microsoft 365 automatically becomes a global administrator.</span></span> <span data-ttu-id="d70f8-151">Глобальный администратор имеет доступ ко всем функциям порталов управления и может:</span><span class="sxs-lookup"><span data-stu-id="d70f8-151">The global admin has access to all features in Management Portals and can:</span></span>

- <span data-ttu-id="d70f8-152">Создание или изменение пользователей</span><span class="sxs-lookup"><span data-stu-id="d70f8-152">Create or edit users</span></span>
- <span data-ttu-id="d70f8-153">Назначение ролей администратора другим лицам</span><span class="sxs-lookup"><span data-stu-id="d70f8-153">Assign admin roles to others</span></span>
- <span data-ttu-id="d70f8-154">Сброс паролей пользователей</span><span class="sxs-lookup"><span data-stu-id="d70f8-154">Reset user passwords</span></span>
- <span data-ttu-id="d70f8-155">Управление пользовательскими лицензиями</span><span class="sxs-lookup"><span data-stu-id="d70f8-155">Manage user licenses</span></span>
- <span data-ttu-id="d70f8-156">Управление доменами</span><span class="sxs-lookup"><span data-stu-id="d70f8-156">Manage domains</span></span>
- <span data-ttu-id="d70f8-157">Утверждение запросов к окнам блокировки клиентов</span><span class="sxs-lookup"><span data-stu-id="d70f8-157">Approve Customer Lockbox requests</span></span>

<span data-ttu-id="d70f8-158">В каждой организации рекомендуется настроить по крайней мере две учетные записи администратора.</span><span class="sxs-lookup"><span data-stu-id="d70f8-158">We recommend that each organization configure at least two admin accounts.</span></span> <span data-ttu-id="d70f8-159">Для крупных предприятий рекомендуется использовать специализированные учетные записи администраторов, которые выполняют различные функции.</span><span class="sxs-lookup"><span data-stu-id="d70f8-159">For large enterprise organizations, we recommend specialized admin accounts that serve different functions.</span></span>

<span data-ttu-id="d70f8-160">Сведения о назначении ролей и разрешений администратора см. в подназначениях ["Назначение](/microsoft-365/admin/add-users/assign-admin-roles) ролей администратора" и ["О ролях администратора".](/microsoft-365/admin/add-users/about-admin-roles)</span><span class="sxs-lookup"><span data-stu-id="d70f8-160">For information about assigning admin roles and permissions, see [Assign admin roles](/microsoft-365/admin/add-users/assign-admin-roles) and [About admin roles](/microsoft-365/admin/add-users/about-admin-roles).</span></span>

## <a name="related-links"></a><span data-ttu-id="d70f8-161">Дополнительные ссылки</span><span class="sxs-lookup"><span data-stu-id="d70f8-161">Related Links</span></span>

- [<span data-ttu-id="d70f8-162">Изоляция в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d70f8-162">Isolation in Microsoft 365</span></span>](assurance-isolation-in-microsoft-365.md)
- [<span data-ttu-id="d70f8-163">Проверка перед трудоустройством в корпорацию Майкрософт</span><span class="sxs-lookup"><span data-stu-id="d70f8-163">Microsoft pre-employment screening</span></span>](assurance-pre-employment-screening.md)
- [<span data-ttu-id="d70f8-164">Фоновая проверка облака Microsoft</span><span class="sxs-lookup"><span data-stu-id="d70f8-164">Microsoft cloud background check</span></span>](assurance-cloud-background-check.md)
- [<span data-ttu-id="d70f8-165">Элементы управления доступом к мониторингу и аудиту</span><span class="sxs-lookup"><span data-stu-id="d70f8-165">Monitoring and Auditing Access Controls</span></span>](assurance-monitoring-and-auditing-access-controls.md)
- [<span data-ttu-id="d70f8-166">Элементы управления доступом к Yammer корпоративный</span><span class="sxs-lookup"><span data-stu-id="d70f8-166">Yammer Enterprise Access Controls</span></span>](assurance-yammer-enterprise-access-controls.md)
