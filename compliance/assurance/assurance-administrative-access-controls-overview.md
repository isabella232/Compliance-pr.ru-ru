---
title: Управление административным доступом в Microsoft 365
description: В этой статье представлен обзор элементов управления административным доступом и классификации данных в Microsoft 365.
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
hideEdit: true
ms.openlocfilehash: e7dc9d73b6eb1961387d85910bb558e85498ffae
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51497705"
---
# <a name="administrative-access-controls-in-microsoft-365"></a><span data-ttu-id="6a095-103">Управление административным доступом в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6a095-103">Administrative access controls in Microsoft 365</span></span> 

<span data-ttu-id="6a095-104">Корпорация Майкрософт инвестировала значительные средства в системы и элементы управления, которые автоматизировали большинство операций Microsoft 365, намеренно ограничив доступ к содержимому клиента корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6a095-104">Microsoft has invested heavily in systems and controls that automate most Microsoft 365 operations while intentionally limiting access to customer content by Microsoft.</span></span> <span data-ttu-id="6a095-105">Люди управляют службой, а программное обеспечение управляет службой.</span><span class="sxs-lookup"><span data-stu-id="6a095-105">Humans govern the service, and software operates the service.</span></span> <span data-ttu-id="6a095-106">Эта структура позволяет Корпорации Майкрософт управлять Microsoft 365 в масштабе и управлять рисками внутренних угроз для контента клиента.</span><span class="sxs-lookup"><span data-stu-id="6a095-106">This structure enables Microsoft to manage Microsoft 365 at scale and manage the risks of internal threats to customer content.</span></span>

<span data-ttu-id="6a095-107">По умолчанию инженеры Майкрософт имеют нулевые административные привилегии и нулевой постоянный доступ к контенту клиента в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6a095-107">By default, Microsoft engineers have zero standing administrative privileges and zero standing access to customer content in Microsoft 365.</span></span> <span data-ttu-id="6a095-108">Инженер Майкрософт может иметь ограниченный, проверенный и защищенный доступ к содержимому клиента в течение ограниченного времени.</span><span class="sxs-lookup"><span data-stu-id="6a095-108">A Microsoft engineer can have limited, audited, and secured access to a customer's content for a limited amount of time.</span></span> <span data-ttu-id="6a095-109">Доступ необходим только при необходимости для операций службы и только в том случае, если он утвержден членом высшего руководства Корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6a095-109">Access is only when necessary for service operations and only when approved by a member of Microsoft senior management.</span></span> <span data-ttu-id="6a095-110">Для клиентов, лицензированных клиентом Lockbox, клиент предоставляет разрешение на доступ к их контенту, который содержится в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6a095-110">For Customer Lockbox licensed customers, the customer provides access approval to their content hosted on Microsoft 365.</span></span>

<span data-ttu-id="6a095-111">Корпорация Майкрософт предоставляет онлайн-службы с использованием нескольких форм облачной доставки:</span><span class="sxs-lookup"><span data-stu-id="6a095-111">Microsoft provides online services using multiple forms of cloud delivery:</span></span>

- <span data-ttu-id="6a095-112">**Общедоступные облака:** Включает несколько версий Microsoft 365, Azure и других служб, которые будут организованы в Северной Америке, Южной Америке, Европе, Азии, Австралии и т.д.</span><span class="sxs-lookup"><span data-stu-id="6a095-112">**Public clouds:** Includes multi-tenant versions of Microsoft 365, Azure, and other services hosted in North America, South America, Europe, Asia, Australia, etc.</span></span>
- <span data-ttu-id="6a095-113">**Национальные облака:** Включает все суверенные и сторонние облака за пределами США (за исключением тех, которые были отмечены ранее), например Microsoft 365 в Китае (управляется 21Vianet) и Microsoft 365 в Германии (управляется Корпорацией Майкрософт, но по модели, в которой немецкий доверитель данных Deutsche Telekom контролирует и контролирует доступ Корпорации Майкрософт к данным клиентов и системам, которые содержат данные клиента).</span><span class="sxs-lookup"><span data-stu-id="6a095-113">**National clouds:** Includes all sovereign and third party-operated clouds outside of the United States (except ones noted previously), such as Microsoft 365 in China (operated by 21Vianet), and Microsoft 365 in Germany (operated by Microsoft, but under a model in which a German data trustee, Deutsche Telekom, controls and monitors Microsoft's access to customer data and systems that contain customer data).</span></span>
- <span data-ttu-id="6a095-114">**Облака правительства:** Включает службы Microsoft 365 и Azure, доступные государственным клиентам США.</span><span class="sxs-lookup"><span data-stu-id="6a095-114">**Government clouds:** Includes Microsoft 365 and Azure services that are available to United States government customers.</span></span>

<span data-ttu-id="6a095-115">Для целей этой статьи службы Microsoft 365 включают:</span><span class="sxs-lookup"><span data-stu-id="6a095-115">For purposes of this article, Microsoft 365 services include:</span></span>

- [<span data-ttu-id="6a095-116">Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6a095-116">Exchange Online</span></span>](/Exchange/exchange-online)
- [<span data-ttu-id="6a095-117">Exchange Online Protection</span><span class="sxs-lookup"><span data-stu-id="6a095-117">Exchange Online Protection</span></span>](/Office365/SecurityCompliance/eop/exchange-online-protection-overview)
- [<span data-ttu-id="6a095-118">SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6a095-118">SharePoint Online</span></span>](/sharepoint/sharepoint-online)
- [<span data-ttu-id="6a095-119">OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="6a095-119">OneDrive for Business</span></span>](/OneDrive/onedrive)
- [<span data-ttu-id="6a095-120">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="6a095-120">Skype for Business</span></span>](/SkypeForBusiness/skype-for-business-online)
- [<span data-ttu-id="6a095-121">Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6a095-121">Microsoft Teams</span></span>](/MicrosoftTeams/Teams-overview)
- [<span data-ttu-id="6a095-122">Yammer</span><span class="sxs-lookup"><span data-stu-id="6a095-122">Yammer</span></span>](/yammer/yammer-landing-page)

## <a name="microsoft-365-access-controls"></a><span data-ttu-id="6a095-123">Элементы управления доступом Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6a095-123">Microsoft 365 access controls</span></span>

<span data-ttu-id="6a095-124">Для целей управления доступом Корпорация Майкрософт классифицировать данные Microsoft 365 в качестве данных клиента или других типов данных.</span><span class="sxs-lookup"><span data-stu-id="6a095-124">For access control purposes, Microsoft categorizes Microsoft 365 data as customer data or other types of data.</span></span>

### <a name="customer-data"></a><span data-ttu-id="6a095-125">Данные клиента</span><span class="sxs-lookup"><span data-stu-id="6a095-125">Customer data</span></span>

<span data-ttu-id="6a095-126">Данные клиента — это все данные, предоставляемые клиентом или от его имени при использовании служб Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6a095-126">Customer data is all data provided by or on behalf of a customer when using Microsoft 365 services.</span></span> <span data-ttu-id="6a095-127">Эти данные — это содержимое клиента, непосредственно созданное или загруженное пользователями Microsoft 365, в том числе:</span><span class="sxs-lookup"><span data-stu-id="6a095-127">This data is customer content directly created or uploaded by Microsoft 365 users, including:</span></span>

- <span data-ttu-id="6a095-128">Сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="6a095-128">Emails</span></span>
- <span data-ttu-id="6a095-129">Контент SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6a095-129">SharePoint Online content</span></span>
- <span data-ttu-id="6a095-130">Мгновенные сообщения</span><span class="sxs-lookup"><span data-stu-id="6a095-130">Instant messages</span></span>
- <span data-ttu-id="6a095-131">Элементы календаря</span><span class="sxs-lookup"><span data-stu-id="6a095-131">Calendar items</span></span>
- <span data-ttu-id="6a095-132">Документы</span><span class="sxs-lookup"><span data-stu-id="6a095-132">Documents</span></span>
- <span data-ttu-id="6a095-133">Контакты</span><span class="sxs-lookup"><span data-stu-id="6a095-133">Contacts</span></span>
- <span data-ttu-id="6a095-134">Идентифицируемая для конечных пользователей информация (EUII) (данные, уникальные для пользователя или связываемые с отдельным пользователем, но не включаемые в содержимое клиента)</span><span class="sxs-lookup"><span data-stu-id="6a095-134">End-user identifiable information (EUII) (data that is unique to a user or that is linkable to an individual user but does not include customer content)</span></span>

### <a name="other-types-of-data"></a><span data-ttu-id="6a095-135">Другие типы данных</span><span class="sxs-lookup"><span data-stu-id="6a095-135">Other types of data</span></span>

<span data-ttu-id="6a095-136">Другие типы данных:</span><span class="sxs-lookup"><span data-stu-id="6a095-136">Other types of data include:</span></span>

- <span data-ttu-id="6a095-137">**Данные учетной записи:** Включает административные данные (сведения, предоставляемые администраторами при регистрации или покупке) и данные платежей (сведения об инструментах оплаты, например сведения о кредитных картах).</span><span class="sxs-lookup"><span data-stu-id="6a095-137">**Account data:** Includes administrative data (information provided by administrators when they sign-up or purchase services), and payment data (information about payment instruments, such as credit card details).</span></span>
- <span data-ttu-id="6a095-138">**Сведения, идентифицируемые с организационной точки зрения:** Включает данные, используемые для идентификации клиента, данные об использовании и не связываемые с отдельным пользователем или включенные в содержимое клиента.</span><span class="sxs-lookup"><span data-stu-id="6a095-138">**Organizationally identifiable information:** Includes data used to identify a tenant, usage data, and not linkable to an individual user or included in customer content.</span></span>
- <span data-ttu-id="6a095-139">**Метаданные системы:** Включает журналы служб, содержащие параметры конфигурации, состояние системы, IP-адреса Microsoft, а также техническую информацию о подписках и клиентах.</span><span class="sxs-lookup"><span data-stu-id="6a095-139">**System metadata:** Includes service logs that contain configuration settings, system status, Microsoft IP addresses, and technical information about subscriptions and tenants.</span></span>

<span data-ttu-id="6a095-140">Корпорация Майкрософт создала механизмы управления доступом, чтобы никто не получил неодобренный доступ к данным клиента или данным управления доступом.</span><span class="sxs-lookup"><span data-stu-id="6a095-140">Microsoft has established access control mechanisms to ensure that no one has unapproved access to Customer Data or access control data.</span></span> <span data-ttu-id="6a095-141">Данные управления доступом управляют доступом к другим типам данных или функций в среде, включая доступ к содержимому клиента или EUII, паролям Майкрософт, сертификатам безопасности и другим данным, связанным с проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="6a095-141">Access control data manages access to other types of data or functions within the environment, including access to customer content or EUII, Microsoft passwords, security certificates, and other authentication-related data.</span></span> <span data-ttu-id="6a095-142">Механизмы управления доступом также не одобряют физический, логический или удаленный доступ к среде производства Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6a095-142">Access control mechanisms also guard against unapproved physical, logical, or remote access to the Microsoft 365 production environment.</span></span>

<span data-ttu-id="6a095-143">Существует три категории элементов управления доступом, используемых Корпорацией Майкрософт для работы с Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="6a095-143">There are three categories of access controls used by Microsoft for operating Microsoft 365:</span></span>

- <span data-ttu-id="6a095-144">Элементы управления изоляцией</span><span class="sxs-lookup"><span data-stu-id="6a095-144">Isolation controls</span></span>
- <span data-ttu-id="6a095-145">Управление персоналом</span><span class="sxs-lookup"><span data-stu-id="6a095-145">Personnel controls</span></span>
- <span data-ttu-id="6a095-146">Технологические элементы управления</span><span class="sxs-lookup"><span data-stu-id="6a095-146">Technology controls</span></span>

<span data-ttu-id="6a095-147">В сочетании эти элементы управления помогают предотвращать и обнаруживать вредоносные действия в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6a095-147">When combined, these controls help prevent and detect malicious actions in Microsoft 365.</span></span> <span data-ttu-id="6a095-148">Помимо элементов управления изоляцией, персоналом и технологиями, используемыми Корпорацией Майкрософт, существует четвертая категория элементов управления: элементы управления, реализуемые клиентами.</span><span class="sxs-lookup"><span data-stu-id="6a095-148">In addition to the isolation, personnel, and technology controls used by Microsoft, there is a fourth category of controls: those controls implemented by customers.</span></span>

<span data-ttu-id="6a095-149">Microsoft 365 позволяет управлять данными так же, как и с данными в локальной среде.</span><span class="sxs-lookup"><span data-stu-id="6a095-149">Microsoft 365 allows you to manage data the same way data is managed in on-premises environments.</span></span> <span data-ttu-id="6a095-150">Человек, подписывавший организацию для Microsoft 365, автоматически становится глобальным администратором.</span><span class="sxs-lookup"><span data-stu-id="6a095-150">The person who signs up an organization for Microsoft 365 automatically becomes a global administrator.</span></span> <span data-ttu-id="6a095-151">Глобальный администратор имеет доступ ко всем функциям порталов управления и может:</span><span class="sxs-lookup"><span data-stu-id="6a095-151">The global admin has access to all features in Management Portals and can:</span></span>

- <span data-ttu-id="6a095-152">Создание или изменение пользователей</span><span class="sxs-lookup"><span data-stu-id="6a095-152">Create or edit users</span></span>
- <span data-ttu-id="6a095-153">Назначение ролей администратора другим</span><span class="sxs-lookup"><span data-stu-id="6a095-153">Assign admin roles to others</span></span>
- <span data-ttu-id="6a095-154">Сброс паролей пользователей</span><span class="sxs-lookup"><span data-stu-id="6a095-154">Reset user passwords</span></span>
- <span data-ttu-id="6a095-155">Управление лицензиями пользователей</span><span class="sxs-lookup"><span data-stu-id="6a095-155">Manage user licenses</span></span>
- <span data-ttu-id="6a095-156">Управление доменами</span><span class="sxs-lookup"><span data-stu-id="6a095-156">Manage domains</span></span>
- <span data-ttu-id="6a095-157">Утверждение запросов на блокировку клиентов</span><span class="sxs-lookup"><span data-stu-id="6a095-157">Approve Customer Lockbox requests</span></span>

<span data-ttu-id="6a095-158">Мы рекомендуем каждой организации настроить по крайней мере две учетные записи администратора.</span><span class="sxs-lookup"><span data-stu-id="6a095-158">We recommend that each organization configure at least two admin accounts.</span></span> <span data-ttu-id="6a095-159">Для крупных организаций мы рекомендуем специализированные учетные записи администратора, которые выполняют различные функции.</span><span class="sxs-lookup"><span data-stu-id="6a095-159">For large enterprise organizations, we recommend specialized admin accounts that serve different functions.</span></span>

<span data-ttu-id="6a095-160">Сведения о назначении ролей и разрешений администратора см. в [рублях Назначение ролей администратора](/microsoft-365/admin/add-users/assign-admin-roles) и [о ролях администратора.](/microsoft-365/admin/add-users/about-admin-roles)</span><span class="sxs-lookup"><span data-stu-id="6a095-160">For information about assigning admin roles and permissions, see [Assign admin roles](/microsoft-365/admin/add-users/assign-admin-roles) and [About admin roles](/microsoft-365/admin/add-users/about-admin-roles).</span></span>

## <a name="related-links"></a><span data-ttu-id="6a095-161">Дополнительные ссылки</span><span class="sxs-lookup"><span data-stu-id="6a095-161">Related Links</span></span>

- [<span data-ttu-id="6a095-162">Изоляция в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6a095-162">Isolation in Microsoft 365</span></span>](assurance-isolation-in-microsoft-365.md)
- [<span data-ttu-id="6a095-163">Проверка перед трудоустройством в корпорацию Майкрософт</span><span class="sxs-lookup"><span data-stu-id="6a095-163">Microsoft pre-employment screening</span></span>](assurance-pre-employment-screening.md)
- [<span data-ttu-id="6a095-164">Фоновая проверка облака Microsoft</span><span class="sxs-lookup"><span data-stu-id="6a095-164">Microsoft cloud background check</span></span>](assurance-cloud-background-check.md)
- [<span data-ttu-id="6a095-165">Элементы управления доступом к мониторингу и аудиту</span><span class="sxs-lookup"><span data-stu-id="6a095-165">Monitoring and Auditing Access Controls</span></span>](assurance-monitoring-and-auditing-access-controls.md)
- [<span data-ttu-id="6a095-166">Элементы управления доступом к Yammer корпоративный</span><span class="sxs-lookup"><span data-stu-id="6a095-166">Yammer Enterprise Access Controls</span></span>](assurance-yammer-enterprise-access-controls.md)
