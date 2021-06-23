---
title: Соображения безопасности и конфиденциальности облачных вычислений правительства Новой Зеландии
description: Корпорация Майкрософт NZ решает вопросы, опубликованные в платформе облачных вычислений Новой Зеландии.
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
ms.openlocfilehash: da53b5e2cdac7095e2fc3ff9b243d2863b85fdbf
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53088788"
---
# <a name="new-zealand-government-cloud-computing-security-and-privacy-considerations"></a><span data-ttu-id="0943d-104">Соображения безопасности и конфиденциальности облачных вычислений правительства Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="0943d-104">New Zealand Government Cloud Computing Security and Privacy Considerations</span></span>

## <a name="new-zealand-government-cloud-computing-security-and-privacy-overview"></a><span data-ttu-id="0943d-105">Обзор безопасности и конфиденциальности облачных вычислений правительства Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="0943d-105">New Zealand Government Cloud Computing Security and Privacy overview</span></span>

<span data-ttu-id="0943d-106">В октябре 2015 г. правительство Новой Зеландии одобрило пересмотренную всеуголную стратегию ИКТ, которая подтвердила свою политику "сначала облака" по использованию информационных технологий в государственном секторе.</span><span class="sxs-lookup"><span data-stu-id="0943d-106">In October 2015, the New Zealand Government endorsed a revised all-government ICT strategy that reaffirmed its 'cloud first' policy on using information technology across the public sector.</span></span> <span data-ttu-id="0943d-107">В пересмотренной стратегии сохраняется "База рисков и гарантий облачных вычислений", которая была разработана и реализована под руководством главного информационного директора правительства Новой Зеландии (GCIO).</span><span class="sxs-lookup"><span data-stu-id="0943d-107">The revised strategy retains the 'Cloud Computing Risk and Assurance Framework' that was developed and implemented under the authority of the NZ Government Chief Information Officer (GCIO).</span></span>

<span data-ttu-id="0943d-108">Правительство ожидает, что все государственные службы Новой Зеландии будут работать в этом рамках при оценке и принятии облачных служб.</span><span class="sxs-lookup"><span data-stu-id="0943d-108">The government expects all New Zealand State Service agencies to work within this framework when assessing and adopting cloud services.</span></span> <span data-ttu-id="0943d-109">В "Требованиях к облачным вычислениям" описывается, что должны делать агентства при принятии облачных служб, а также обзор истории облачной политики правительства.</span><span class="sxs-lookup"><span data-stu-id="0943d-109">'Requirements for Cloud Computing' outlines what agencies must do when adopting cloud services along with an overview of the history of the government's cloud policy.</span></span>

<span data-ttu-id="0943d-110">Чтобы помочь правительственным учреждениям NZ в проведении последовательной и надежной должной осмотрительности потенциальных облачных решений, GCIO опубликовала cloud [Computing: Information Security and Privacy Considerations (ISPC).](https://www.digital.govt.nz/dmsdocument/1~cloud-computing-information-security-and-privacy-considerations/html)</span><span class="sxs-lookup"><span data-stu-id="0943d-110">To assist NZ government agencies in conducting consistent and robust due diligence on potential cloud solutions, the GCIO has published [Cloud Computing: Information Security and Privacy Considerations (ISPC)](https://www.digital.govt.nz/dmsdocument/1~cloud-computing-information-security-and-privacy-considerations/html).</span></span> <span data-ttu-id="0943d-111">В этом документе содержится более 100 вопросов, которые посвящены суверенитету данных, конфиденциальности, безопасности, управлению, конфиденциальности, целостности данных, доступности и реагированию на инциденты и управлению ими.</span><span class="sxs-lookup"><span data-stu-id="0943d-111">This document contains more than 100 questions focused on data sovereignty, privacy, security, governance, confidentiality, data integrity, availability, and incident response and management.</span></span> <span data-ttu-id="0943d-112">IsPC не определяет правительственный стандарт NZ, в соответствии с которым поставщики облачных служб должны демонстрировать формальное соответствие требованиям.</span><span class="sxs-lookup"><span data-stu-id="0943d-112">The ISPC does not define a NZ government standard against which cloud service providers must demonstrate formal compliance.</span></span> <span data-ttu-id="0943d-113">Однако многие из вопросов, задамые в документе, указывают на важность понимания соответствия поставщиков облачных служб широкому спектру соответствующих стандартов.</span><span class="sxs-lookup"><span data-stu-id="0943d-113">Many of the questions set out in the document do, however, point toward the importance of understanding how cloud service providers comply with a wide array of relevant standards.</span></span>

## <a name="microsoft-and-new-zealand-government-cloud-computing-security-and-privacy-considerations"></a><span data-ttu-id="0943d-114">Соображения безопасности и конфиденциальности облачных вычислений корпорации Майкрософт и Правительства Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="0943d-114">Microsoft and New Zealand Government Cloud Computing Security and Privacy Considerations</span></span>

<span data-ttu-id="0943d-115">Чтобы помочь учреждениям в анализе и оценке облачных служб Майкрософт, Корпорация Майкрософт в Новой Зеландии подготовила документы, показывающие, как корпоративные облачные службы отвечают на вопросы, задающиеся в ISPC облачных вычислений, связывая их со стандартами, с которыми сертифицированы облачные службы Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0943d-115">To help agencies undertake their analysis and evaluation of Microsoft enterprise cloud services, Microsoft New Zealand has produced documents showing how its enterprise cloud services address the questions set out in the 'Cloud Computing ISPC' by linking them to the standards against which Microsoft cloud services are certified.</span></span> <span data-ttu-id="0943d-116">Эти сертификаты имеют центральное значение для того, как Корпорация Майкрософт гарантирует клиентам государственного и частного сектора, что ее облачные службы разработаны, построены и работают для эффективного снижения рисков конфиденциальности и безопасности и решения проблем, связанных с суверенитетом данных.</span><span class="sxs-lookup"><span data-stu-id="0943d-116">These certifications are central to how Microsoft assures both public and private sector customers that its cloud services are designed, built, and operated to effectively mitigate privacy and security risks and address data sovereignty concerns.</span></span> <span data-ttu-id="0943d-117">Для скачивания пользователям доступен ответ Azure на [ISPC](https://azure.microsoft.com/resources/microsoft-azure-response-to-nz-gcio-cloud-computing-information-security-privacy-considerations/) облачных вычислений.</span><span class="sxs-lookup"><span data-stu-id="0943d-117">The [Azure response to Cloud Computing ISPC](https://azure.microsoft.com/resources/microsoft-azure-response-to-nz-gcio-cloud-computing-information-security-privacy-considerations/) is available to customers for download.</span></span>

## <a name="microsoft-in-scope-cloud-services"></a><span data-ttu-id="0943d-118">Облачные службы Майкрософт, к которым применима оценка</span><span class="sxs-lookup"><span data-stu-id="0943d-118">Microsoft in-scope cloud services</span></span>

- [<span data-ttu-id="0943d-119">Azure и Azure для государственных организаций</span><span class="sxs-lookup"><span data-stu-id="0943d-119">Azure and Azure Government</span></span>](https://aka.ms/AzureCompliance)
- [<span data-ttu-id="0943d-120">Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="0943d-120">Dynamics 365</span></span>](https://aka.ms/d365-compliance-list)
- <span data-ttu-id="0943d-121">Intune</span><span class="sxs-lookup"><span data-stu-id="0943d-121">Intune</span></span>
- <span data-ttu-id="0943d-122">Облачная служба Power BI в виде автономной службы или в составе плана либо набора Office 365</span><span class="sxs-lookup"><span data-stu-id="0943d-122">Power BI cloud service either as a standalone service or as included in an Office 365 branded plan or suite</span></span>
- [<span data-ttu-id="0943d-123">Office 365</span><span class="sxs-lookup"><span data-stu-id="0943d-123">Office 365</span></span>](https://go.microsoft.com/fwlink/p/?LinkID=2077751)
- <span data-ttu-id="0943d-124">Exchange Online, SharePoint Online и Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0943d-124">Exchange Online, SharePoint Online, and Microsoft Teams.</span></span> <span data-ttu-id="0943d-125">Корпорация Майкрософт NZ сотрудничала с командой GCIO для разработки эталонной архитектуры для интеграции Exchange Online SEEMail.</span><span class="sxs-lookup"><span data-stu-id="0943d-125">Microsoft NZ has worked with the GCIO team to develop a reference architecture for integrating Exchange Online and SEEMail.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="0943d-126">Вопросы и ответы</span><span class="sxs-lookup"><span data-stu-id="0943d-126">Frequently asked questions</span></span>

<span data-ttu-id="0943d-127">**К кому применяется эта структура?**</span><span class="sxs-lookup"><span data-stu-id="0943d-127">**To whom does the framework apply?**</span></span>

<span data-ttu-id="0943d-128">Организации, подпадающие под мандат GCIO, государственные и негосударственные службы, 20 окружных советов здравоохранения и 7 субъектов Короны, должны придерживаться этой структуры при принятии решения об использовании облачной службы.</span><span class="sxs-lookup"><span data-stu-id="0943d-128">Organizations that fall under the GCIO mandate, the public and non-public service departments, the 20 district health boards, and 7 Crown entities, must adhere to the framework when they are deciding on the use of a cloud service.</span></span>

<span data-ttu-id="0943d-129">**Может ли мое агентство использовать ответы Корпорации Майкрософт на эти рамки в процессе сертификации наших систем ИКТ?**</span><span class="sxs-lookup"><span data-stu-id="0943d-129">**Can my agency use Microsoft's responses to this framework in the certification process of our ICT systems?**</span></span>

<span data-ttu-id="0943d-130">Если ваше агентство обязано проводить сертификацию и аккредитацию своей системы ИКТ в руководстве по информационной безопасности Новой [Зеландии,](https://go.microsoft.com/fwlink/p/?linkid=2099496)вы можете использовать эти ответы в рамках анализа.</span><span class="sxs-lookup"><span data-stu-id="0943d-130">If your agency is required to undertake certification and accreditation of its ICT system under the [New Zealand Information Security Manual](https://go.microsoft.com/fwlink/p/?linkid=2099496), then you can use these responses as part of your analysis.</span></span>

## <a name="resources"></a><span data-ttu-id="0943d-131">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="0943d-131">Resources</span></span>

- [<span data-ttu-id="0943d-132">Требования к безопасности для офшорных служб Office производительности: руководство по соответствунию для Office 365</span><span class="sxs-lookup"><span data-stu-id="0943d-132">Security requirements for offshore hosted Office productivity services: conformance guide for Office 365</span></span>](https://aka.ms/o365-gcio-conformance-guidance)
- [<span data-ttu-id="0943d-133">Стратегия ИКТ правительства NZ 2015</span><span class="sxs-lookup"><span data-stu-id="0943d-133">NZ Government ICT Strategy 2015</span></span>](https://www.ict.govt.nz/strategy-and-action-plan/strategy/)
- [<span data-ttu-id="0943d-134">Облачные вычисления: соображения информационной безопасности и конфиденциальности (ISPC)</span><span class="sxs-lookup"><span data-stu-id="0943d-134">Cloud Computing: Information Security and Privacy Considerations (ISPC)</span></span>](https://www.digital.govt.nz/standards-and-guidance/technology-and-architecture/cloud-services/)
- [<span data-ttu-id="0943d-135">Условия использования веб-служб Майкрософт</span><span class="sxs-lookup"><span data-stu-id="0943d-135">Microsoft Online Services Terms</span></span>](https://aka.ms/Online-Services-Terms)
- [<span data-ttu-id="0943d-136">Соответствие требованиям в центре управления безопасностью Майкрософт</span><span class="sxs-lookup"><span data-stu-id="0943d-136">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)

## <a name="microsoft-responses-to-cloud-computing-ipsc"></a><span data-ttu-id="0943d-137">Ответы Корпорации Майкрософт на IPSC облачных вычислений</span><span class="sxs-lookup"><span data-stu-id="0943d-137">Microsoft responses to 'Cloud Computing IPSC'</span></span>

- [<span data-ttu-id="0943d-138">Azure</span><span class="sxs-lookup"><span data-stu-id="0943d-138">Azure</span></span>](https://aka.ms/Azure-NZ-response)
- [<span data-ttu-id="0943d-139">Intune</span><span class="sxs-lookup"><span data-stu-id="0943d-139">Intune</span></span>](https://aka.ms/Intune-NZ-response)
- [<span data-ttu-id="0943d-140">Office 365</span><span class="sxs-lookup"><span data-stu-id="0943d-140">Office 365</span></span>](https://aka.ms/O365-NZ-Response)
- [<span data-ttu-id="0943d-141">Power BI</span><span class="sxs-lookup"><span data-stu-id="0943d-141">Power BI</span></span>](https://download.microsoft.com/download/5/1/7/51726B9B-2E76-49C4-9D4F-A36BF025CB93/Response-to-GCIO-105-questions-Power-BI.pdf)
