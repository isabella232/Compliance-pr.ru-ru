---
title: Уровень воздействия Министерства обороны (DoD) 2 (IL2)
description: Узнайте, как Корпорация Майкрософт отвечает стандартам 2 (IL2) для Министерства обороны (DoD).
keywords: Microsoft 365, соответствие требованиям, предложения
localization_priority: None
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmazz
manager: laurawi
audience: itpro
ms.collection:
- M365-security-compliance
- MS-Compliance
hideEdit: true
titleSuffix: Microsoft Compliance
ms.openlocfilehash: 77e8cb50f815c167e50293d495b4a548a73d022e
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2021
ms.locfileid: "53385755"
---
# <a name="department-of-defense-dod-impact-level-2-il2"></a><span data-ttu-id="2e329-104">Уровень воздействия Министерства обороны (DoD) 2 (IL2)</span><span class="sxs-lookup"><span data-stu-id="2e329-104">Department of Defense (DoD) Impact Level 2 (IL2)</span></span>

## <a name="dod-il2-overview"></a><span data-ttu-id="2e329-105">Обзор DoD IL2</span><span class="sxs-lookup"><span data-stu-id="2e329-105">DoD IL2 overview</span></span>

<span data-ttu-id="2e329-106">Агентство информационных систем обороны (DISA) — это агентство Министерства обороны США, которое отвечает за разработку и обслуживание руководства по безопасности облачных вычислений DoD [(SRG).](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)</span><span class="sxs-lookup"><span data-stu-id="2e329-106">The Defense Information Systems Agency (DISA) is an agency of the US Department of Defense (DoD) that is responsible for developing and maintaining the DoD Cloud Computing [Security Requirements Guide (SRG)](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html).</span></span> <span data-ttu-id="2e329-107">SRG определяет базовые требования к безопасности, используемые DoD для оценки позиции безопасности поставщика облачных служб (CSP), поддерживающих решение о предоставлении предварительной авторизации (PA) DoD, которая позволяет CSP принимать миссии DoD.</span><span class="sxs-lookup"><span data-stu-id="2e329-107">The SRG defines the baseline security requirements used by DoD to assess the security posture of a cloud service provider (CSP), supporting the decision to grant a DoD Provisional Authorization (PA) that allows a CSP to host DoD missions.</span></span> <span data-ttu-id="2e329-108">Он включает, заметив и отменить ранее опубликованную модель облачной безопасности DoD (CSM) и карты в Рамках управления рисками DoD (RMF).</span><span class="sxs-lookup"><span data-stu-id="2e329-108">It incorporates, supersedes, and rescinds the previously published DoD Cloud Security Model (CSM) and maps to the DoD Risk Management Framework (RMF).</span></span>

<span data-ttu-id="2e329-109">DISA направляет агентства и отделы Министерства обороны в планировании и санкционировании использования CSP.</span><span class="sxs-lookup"><span data-stu-id="2e329-109">DISA guides DoD agencies and departments in planning and authorizing the use of a CSP.</span></span> <span data-ttu-id="2e329-110">Он также оценивает предложения CSP на соответствие SRG , процесс авторизации, в соответствии с которой CSPs может предоставлять документацию, из которой следует, что они соответствует стандартам DoD.</span><span class="sxs-lookup"><span data-stu-id="2e329-110">It also evaluates CSP offerings for compliance with the SRG, an authorization process whereby CSPs can furnish documentation outlining their compliance with DoD standards.</span></span> <span data-ttu-id="2e329-111">При необходимости он выдает временные разрешения doD, поэтому агентства doD и поддерживающие организации могут использовать облачные службы без необходимости самостоятельного полного утверждения, экономя время и усилия.</span><span class="sxs-lookup"><span data-stu-id="2e329-111">It issues DoD Provisional Authorizations (PAs) when appropriate, so DoD agencies and supporting organizations can use cloud services without having to go through a full approval process on their own, saving time and effort.</span></span>

<span data-ttu-id="2e329-112">В памятке doD CIO от 15 декабря  [2014](https://www.esi.mil/contentview.aspx?id=585) г. о обновленных руководствах по приобретению и использованию коммерческих облачных вычислительных служб говорится, что "FedRAMP будет служить минимальным базовым уровнем безопасности для всех облачных служб DoD".</span><span class="sxs-lookup"><span data-stu-id="2e329-112">The [15 December 2014 DoD CIO memo](https://www.esi.mil/contentview.aspx?id=585) regarding *Updated Guidance on the Acquisition and Use of Commercial Cloud Computing Services* states that 'FedRAMP will serve as the minimum security baseline for all DoD cloud services'.</span></span> <span data-ttu-id="2e329-113">SRG использует базовую линию FedRAMP Moderate на всех уровнях влияния информации (IL) и рассматривает высокий базовый уровень в некоторых случаях.</span><span class="sxs-lookup"><span data-stu-id="2e329-113">The SRG uses the FedRAMP Moderate baseline at all information impact levels (IL) and considers the High Baseline at some.</span></span>

<span data-ttu-id="2e329-114">В разделе [SRG 5.1.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) DoD управления безопасностью *FedRAMP* говорится, что информация IL2 может быть организована в CSP, где минимально имеется умеренный PA FedRAMP и PA уровня DoD 2 при условии соблюдения требований безопасности персонала, изложенных в разделе 5.6.2.</span><span class="sxs-lookup"><span data-stu-id="2e329-114">[SRG Section 5.1.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD use of FedRAMP Security Controls* states that IL2 information may be hosted in a CSP that minimally holds a FedRAMP Moderate PA and a DoD Level 2 PA, subject to compliance with the personnel security requirements outlined in Section 5.6.2.</span></span> <span data-ttu-id="2e329-115">Однако этот подход не облегчает CSP другие требования к безопасности и интеграции, как того требует владелец миссии.</span><span class="sxs-lookup"><span data-stu-id="2e329-115">However, this approach does not alleviate the CSP from meeting other security and integration requirements as required by the Mission Owner.</span></span> <span data-ttu-id="2e329-116">Согласно [SRG Section 5.2.2.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5.2LegalConsiderations) IL2 Location *and Separation Requirements,* DOD IL2 PA адекватно покрывается pa FedRAMP Moderate, чтобы требования не были дополнительно оценены для PA IL2.</span><span class="sxs-lookup"><span data-stu-id="2e329-116">According to [SRG Section 5.2.2.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5.2LegalConsiderations) *IL2 Location and Separation Requirements*, DoD IL2 PA is adequately covered by a FedRAMP Moderate PA such that the requirements will not be additionally assessed for an IL2 PA.</span></span>

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="2e329-117">Облачные платформы Microsoft в области & служб</span><span class="sxs-lookup"><span data-stu-id="2e329-117">Microsoft in-scope cloud platforms & services</span></span>

- <span data-ttu-id="2e329-118">Azure</span><span class="sxs-lookup"><span data-stu-id="2e329-118">Azure</span></span>
- <span data-ttu-id="2e329-119">Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="2e329-119">Dynamics 365</span></span>
- <span data-ttu-id="2e329-120">Microsoft Cloud App Security</span><span class="sxs-lookup"><span data-stu-id="2e329-120">Microsoft Cloud App Security</span></span>
- <span data-ttu-id="2e329-121">Microsoft Defender для конечной точки</span><span class="sxs-lookup"><span data-stu-id="2e329-121">Microsoft Defender for Endpoint</span></span>
- <span data-ttu-id="2e329-122">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e329-122">Microsoft Graph</span></span>
- <span data-ttu-id="2e329-123">Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2e329-123">Microsoft Intune</span></span>
- <span data-ttu-id="2e329-124">Microsoft Stream</span><span class="sxs-lookup"><span data-stu-id="2e329-124">Microsoft Stream</span></span>
- <span data-ttu-id="2e329-125">Office 365 Правительство США, Office 365 правительство США - Высокая</span><span class="sxs-lookup"><span data-stu-id="2e329-125">Office 365 U.S. Government, Office 365 U.S. Government - High</span></span>
- <span data-ttu-id="2e329-126">Power Apps</span><span class="sxs-lookup"><span data-stu-id="2e329-126">Power Apps</span></span>
- <span data-ttu-id="2e329-127">Power Automate</span><span class="sxs-lookup"><span data-stu-id="2e329-127">Power Automate</span></span>
- <span data-ttu-id="2e329-128">Power BI</span><span class="sxs-lookup"><span data-stu-id="2e329-128">Power BI</span></span>

## <a name="azure-dynamics-365-and-dod-il2"></a><span data-ttu-id="2e329-129">Azure, Dynamics 365 и DoD IL2</span><span class="sxs-lookup"><span data-stu-id="2e329-129">Azure, Dynamics 365, and DoD IL2</span></span>

<span data-ttu-id="2e329-130">Дополнительные сведения о соответствии Azure, Dynamics 365 и другим сетевым службам см. в предложении [Azure DoD IL2.](/azure/compliance/offerings/offering-dod-il2)</span><span class="sxs-lookup"><span data-stu-id="2e329-130">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure DoD IL2 offering](/azure/compliance/offerings/offering-dod-il2).</span></span>

## <a name="office-365-and-dod-il2"></a><span data-ttu-id="2e329-131">Office 365 и DoD IL2</span><span class="sxs-lookup"><span data-stu-id="2e329-131">Office 365 and DoD IL2</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="2e329-132">Office 365 облачных сред</span><span class="sxs-lookup"><span data-stu-id="2e329-132">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="2e329-133">Office 365 и службы в области применения</span><span class="sxs-lookup"><span data-stu-id="2e329-133">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="2e329-134">Используйте следующую таблицу, чтобы определить применимость для Office 365 и подписки:</span><span class="sxs-lookup"><span data-stu-id="2e329-134">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="2e329-135">**Применимость**</span><span class="sxs-lookup"><span data-stu-id="2e329-135">**Applicability**</span></span> | <span data-ttu-id="2e329-136">**In-scope services**</span><span class="sxs-lookup"><span data-stu-id="2e329-136">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="2e329-137">**GCC**</span><span class="sxs-lookup"><span data-stu-id="2e329-137">**GCC**</span></span> | <span data-ttu-id="2e329-138">Служба каналов активности, службы Bing, Delve, Exchange Online Protection, Exchange Online, интеллектуальные службы, Microsoft Teams, Office 365 клиентский портал, Office Online, инфраструктура Office, Office Отчеты об использовании, OneDrive для бизнеса, Карточка людей, SharePoint Online, Skype для бизнеса, Windows Ink</span><span class="sxs-lookup"><span data-stu-id="2e329-138">Activity Feed Service, Bing Services, Delve, Exchange Online Protection, Exchange Online, Intelligent Services, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, SharePoint Online, Skype for Business, Windows Ink</span></span> |
| <span data-ttu-id="2e329-139">**GCC High**</span><span class="sxs-lookup"><span data-stu-id="2e329-139">**GCC High**</span></span> | <span data-ttu-id="2e329-140">Служба каналов активности, службы Bing, Delve, Exchange Online Protection, Exchange Online, интеллектуальные службы, Microsoft Teams, Office 365 клиентский портал, Office Online, инфраструктура Office, Office Отчеты об использовании, OneDrive для бизнеса, Карточка людей, SharePoint Online, Skype для бизнеса, Windows Ink</span><span class="sxs-lookup"><span data-stu-id="2e329-140">Activity Feed Service, Bing Services, Delve, Exchange Online Protection, Exchange Online, Intelligent Services, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, SharePoint Online, Skype for Business, Windows Ink</span></span> |

### <a name="resources"></a><span data-ttu-id="2e329-141">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="2e329-141">Resources</span></span>

- [<span data-ttu-id="2e329-142">Решения для правительства Майкрософт</span><span class="sxs-lookup"><span data-stu-id="2e329-142">Microsoft government solutions</span></span>](https://www.microsoft.com/enterprise/government)
- [<span data-ttu-id="2e329-143">Руководство по обеспечению безопасности облачных вычислений DoD</span><span class="sxs-lookup"><span data-stu-id="2e329-143">DoD Cloud Computing Security Requirements Guide</span></span>](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)
- [<span data-ttu-id="2e329-144">Документы FedRAMP</span><span class="sxs-lookup"><span data-stu-id="2e329-144">FedRAMP documents</span></span>](https://www.fedramp.gov/documents/)
- <span data-ttu-id="2e329-145">База управления рисками для информационных систем и организаций [NIST SP 800-37:](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) системный подход Life-Cycle безопасности *и конфиденциальности*</span><span class="sxs-lookup"><span data-stu-id="2e329-145">[NIST SP 800-37](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) *Risk Management Framework for Information Systems and Organizations: A System Life-Cycle Approach for Security and Privacy*</span></span>
- <span data-ttu-id="2e329-146">[NIST SP 800-53](https://csrc.nist.gov/Projects/risk-management/sp800-53-controls/release-search#!/800-53) Управление безопасностью и *конфиденциальностью для информационных систем и организаций*</span><span class="sxs-lookup"><span data-stu-id="2e329-146">[NIST SP 800-53](https://csrc.nist.gov/Projects/risk-management/sp800-53-controls/release-search#!/800-53) *Security and Privacy Controls for Information Systems and Organizations*</span></span>
- <span data-ttu-id="2e329-147">[Инструкция DoD 8510.01](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodi/851001p.pdf) *DoD Risk Management Framework (RMF)* для информационных технологий DoD (IT)</span><span class="sxs-lookup"><span data-stu-id="2e329-147">[DoD Instruction 8510.01](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodi/851001p.pdf) *DoD Risk Management Framework (RMF) for DoD Information Technology (IT)*</span></span>
