---
title: ISO/IEC 27017:2015 "Свод правил по управлению информационной безопасностью"
description: В облачных службах Майкрософт реализованы этот свод правил по управлению информационной безопасностью.
keywords: Microsoft 365, соответствие требованиям, предложения
localization_priority: Priority
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
ms.openlocfilehash: 09473dc7b27b34bd4b0394739cd303fa613780bf
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51497740"
---
# <a name="isoiec-270172015-code-of-practice-for-information-security-controls"></a><span data-ttu-id="646bd-104">ISO/IEC 27017:2015 "Свод правил по управлению информационной безопасностью"</span><span class="sxs-lookup"><span data-stu-id="646bd-104">ISO/IEC 27017:2015 Code of Practice for Information Security Controls</span></span>

## <a name="iso-iec-27017-overview"></a><span data-ttu-id="646bd-105">Общие сведения о ISO-IEC 27017</span><span class="sxs-lookup"><span data-stu-id="646bd-105">ISO-IEC 27017 Overview</span></span>

<span data-ttu-id="646bd-106">Свод правил ISO/IEC 27017:2015 предназначен для организаций для использования в качестве справочника при выборе средств контроля информационной безопасностью облачных служб при реализации системы управления информационной безопасностью облачных вычислений на основе стандарта ISO/IEC 27002:2013.</span><span class="sxs-lookup"><span data-stu-id="646bd-106">The ISO/IEC 27017:2015 code of practice is designed for organizations to use as a reference for selecting cloud services information security controls when implementing a cloud computing information security management system based on ISO/IEC 27002:2013.</span></span> <span data-ttu-id="646bd-107">Он также может использоваться поставщиками облачных служб в качестве руководства по реализации общепринятых средств контроля защиты.</span><span class="sxs-lookup"><span data-stu-id="646bd-107">It can also be used by cloud service providers as a guidance document for implementing commonly accepted protection controls.</span></span>

<span data-ttu-id="646bd-108">Этот международный стандарт предоставляет дополнительные инструкции по внедрению для облачной среды, основанные на стандарте ISO/IEC 27002, и содержит дополнительные средства контроля для устранения облачных рисков и угроз информационной безопасности, ссылаясь на пункты 5-18 стандарта ISO/IEC 27002:2013 со сведениями об средствах контроля, инструкциями реализации и прочей информацией.</span><span class="sxs-lookup"><span data-stu-id="646bd-108">This international standard provides additional cloud-specific implementation guidance based on ISO/IEC 27002, and provides additional controls to address cloud-specific information security threats and risks referring to clauses 5-18 in ISO/IEC 27002: 2013 for controls, implementation guidance, and other information.</span></span> <span data-ttu-id="646bd-109">В частности, этот стандарт предоставляет инструкции по 37 средствам контроля из стандарта ISO/IEC 27002, а также содержит семь новых средств контроля, отсутствующих в стандарте ISO/IEC 27002.</span><span class="sxs-lookup"><span data-stu-id="646bd-109">Specifically, this standard provides guidance on 37 controls in ISO/IEC 27002, and it also features seven new controls that are not duplicated in ISO/IEC 27002.</span></span> <span data-ttu-id="646bd-110">Эти новые средства контроля предназначены для следующих важных областей:</span><span class="sxs-lookup"><span data-stu-id="646bd-110">These new controls address the following important areas:</span></span>

- <span data-ttu-id="646bd-111">Общие роли и обязанности в облачной среде</span><span class="sxs-lookup"><span data-stu-id="646bd-111">Shared roles and responsibilities within a cloud computing environment</span></span>
- <span data-ttu-id="646bd-112">Удаление и возврат ресурсов клиента облачной службы при расторжении договора</span><span class="sxs-lookup"><span data-stu-id="646bd-112">Removal and return of cloud service customer assets upon contract termination</span></span>
- <span data-ttu-id="646bd-113">Защита и отделение виртуальной среды клиента от сред других клиентов</span><span class="sxs-lookup"><span data-stu-id="646bd-113">Protection and separation of a customer's virtual environment from environments of other customers</span></span>
- <span data-ttu-id="646bd-114">Требования к обеспечению безопасности виртуальной машины для соблюдения бизнес-потребностей</span><span class="sxs-lookup"><span data-stu-id="646bd-114">Virtual machine hardening requirements to meet business needs</span></span>
- <span data-ttu-id="646bd-115">Процедуры для административных операций с облачной средой</span><span class="sxs-lookup"><span data-stu-id="646bd-115">Procedures for administrative operations of a cloud computing environment</span></span>
- <span data-ttu-id="646bd-116">Разрешение клиентам отслеживать важные действия в облачной среде</span><span class="sxs-lookup"><span data-stu-id="646bd-116">Enabling customers to monitor relevant activities within a cloud computing environment</span></span>
- <span data-ttu-id="646bd-117">Согласование управления безопасностью для виртуальных и физических сетей</span><span class="sxs-lookup"><span data-stu-id="646bd-117">Alignment of security management for virtual and physical networks</span></span>

## <a name="microsoft-and-isoiec-27017"></a><span data-ttu-id="646bd-118">Майкрософт и ISO/IEC 27017</span><span class="sxs-lookup"><span data-stu-id="646bd-118">Microsoft and ISO/IEC 27017</span></span>

<span data-ttu-id="646bd-119">ISO/IEC 27017 является уникальным стандартом, предоставляющим руководство как поставщикам облачных служб, так и клиентам облачных служб.</span><span class="sxs-lookup"><span data-stu-id="646bd-119">ISO/IEC 27017 is unique in providing guidance for both cloud service providers and cloud service customers.</span></span> <span data-ttu-id="646bd-120">Он также содержит практические сведения для клиентов облачных служб о том, что следует ожидать от поставщиков облачных служб.</span><span class="sxs-lookup"><span data-stu-id="646bd-120">It also provides cloud service customers with practical information on what they should expect from cloud service providers.</span></span> <span data-ttu-id="646bd-121">Клиенты могут получить прямую выгоду от использования стандарта ISO/IEC 27017, разобравшись с понятием общей ответственности в облаке.</span><span class="sxs-lookup"><span data-stu-id="646bd-121">Customers can benefit directly from ISO/IEC 27017 by ensuring they understand the shared responsibilities in the cloud.</span></span>

## <a name="microsoft-in-scope-cloud-services"></a><span data-ttu-id="646bd-122">Облачные службы Майкрософт, к которым применима оценка</span><span class="sxs-lookup"><span data-stu-id="646bd-122">Microsoft in-scope cloud services</span></span>

- [<span data-ttu-id="646bd-123">Azure, Azure для государственных организаций и Azure для Германии</span><span class="sxs-lookup"><span data-stu-id="646bd-123">Azure, Azure Government, and Azure Germany</span></span>](https://aka.ms/AzureCompliance)
- <span data-ttu-id="646bd-124">Microsoft Cloud App Security</span><span class="sxs-lookup"><span data-stu-id="646bd-124">Microsoft Cloud App Security</span></span>
- [<span data-ttu-id="646bd-125">Dynamics 365, Dynamics 365 для государственных учреждений и Dynamics 365 — Германия</span><span class="sxs-lookup"><span data-stu-id="646bd-125">Dynamics 365, Dynamics 365, and Dynamics 365 Germany</span></span>](https://aka.ms/d365-compliance-list)
- <span data-ttu-id="646bd-126">Microsoft Defender для конечной точки</span><span class="sxs-lookup"><span data-stu-id="646bd-126">Microsoft Defender for Endpoint</span></span>
- <span data-ttu-id="646bd-127">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="646bd-127">Microsoft Graph</span></span>
- <span data-ttu-id="646bd-128">Microsoft Healthcare Bot</span><span class="sxs-lookup"><span data-stu-id="646bd-128">Microsoft Healthcare Bot</span></span>
- <span data-ttu-id="646bd-129">Intune</span><span class="sxs-lookup"><span data-stu-id="646bd-129">Intune</span></span>
- [<span data-ttu-id="646bd-130">Компьютеры, управляемые Майкрософт</span><span class="sxs-lookup"><span data-stu-id="646bd-130">Microsoft Managed Desktop</span></span>](/microsoft-365/managed-desktop/intro/compliance)
- <span data-ttu-id="646bd-131">Облачная служба Power Automate (прежнее название Microsoft Flow) в виде автономной службы или в составе плана либо набора Office 365 или Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="646bd-131">Power Automate (formerly Microsoft Flow) cloud service either as a standalone service or as included in an Office 365 or Dynamics 365 branded plan or suite</span></span>
- <span data-ttu-id="646bd-132">Office 365, Office 365 для государственных организаций США, Office 365 U.S. Government Defense и Office 365 Germany</span><span class="sxs-lookup"><span data-stu-id="646bd-132">Office 365, Office 365 U.S. Government, Office 365 U.S. Government Defense, and Office 365 Germany</span></span>
- <span data-ttu-id="646bd-133">Облачная служба PowerApps в виде автономной службы или в составе плана либо набора Office 365 или Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="646bd-133">PowerApps cloud service either as a standalone service or as included in an Office 365 or Dynamics 365 branded plan or suite</span></span>
- <span data-ttu-id="646bd-134">Облачная служба Power BI в виде автономной службы или в составе плана либо набора Office 365</span><span class="sxs-lookup"><span data-stu-id="646bd-134">Power BI cloud service either as a standalone service or as included in an Office 365 branded plan or suite</span></span>
- <span data-ttu-id="646bd-135">Power BI Embedded</span><span class="sxs-lookup"><span data-stu-id="646bd-135">Power BI Embedded</span></span>
- <span data-ttu-id="646bd-136">Microsoft Stream</span><span class="sxs-lookup"><span data-stu-id="646bd-136">Microsoft Stream</span></span>
- <span data-ttu-id="646bd-137">Ознакомьтесь с [подробным списком](https://go.microsoft.com/fwlink/p/?linkid=2077751) поддерживаемых служб в Office 365</span><span class="sxs-lookup"><span data-stu-id="646bd-137">See a [detailed list](https://go.microsoft.com/fwlink/p/?linkid=2077751) of covered services in Office 365</span></span>

## <a name="audits-reports-and-certificates"></a><span data-ttu-id="646bd-138">Аудит, отчеты и сертификаты</span><span class="sxs-lookup"><span data-stu-id="646bd-138">Audits, reports, and certificates</span></span>

<span data-ttu-id="646bd-139">Аудит облачных служб Майкрософт выполняется раз в год на соответствие своду правил ISO/IEC 27017:2015 в рамках процесса сертификации для ISO/IEC 27001:2013.</span><span class="sxs-lookup"><span data-stu-id="646bd-139">Microsoft cloud services are audited once a year for the ISO/IEC 27017:2015 code of practice as part of the certification process for ISO/IEC 27001:2013.</span></span>

- [<span data-ttu-id="646bd-140">Сертификат Azure ISO 27017</span><span class="sxs-lookup"><span data-stu-id="646bd-140">Azure ISO 27017 Certificate</span></span>](https://aka.ms/azureiso27017cert)
- [<span data-ttu-id="646bd-141">Отчет по оценке Azure ISO 27017</span><span class="sxs-lookup"><span data-stu-id="646bd-141">Azure ISO 27017 Assessment report</span></span>](https://aka.ms/azureiso27017report)
- [<span data-ttu-id="646bd-142">Office 365: отчет об оценке аудита ISO 27001, 27018 и 27017</span><span class="sxs-lookup"><span data-stu-id="646bd-142">Office 365: ISO 27001, 27018, and 27017 Audit Assessment Report</span></span>](https://aka.ms/o365isoreport)

## <a name="frequently-asked-questions"></a><span data-ttu-id="646bd-143">Вопросы и ответы</span><span class="sxs-lookup"><span data-stu-id="646bd-143">Frequently asked questions</span></span>

<span data-ttu-id="646bd-144">К кому применим стандарт?</span><span class="sxs-lookup"><span data-stu-id="646bd-144">To whom does the standard apply?</span></span>

<span data-ttu-id="646bd-145">Этот свод правил содержит средства контроля и инструкции по реализации для поставщиков облачных служб и клиентов облачных служб.</span><span class="sxs-lookup"><span data-stu-id="646bd-145">This code of practice provides controls and implementation guidance for both cloud service providers and cloud service customers.</span></span> <span data-ttu-id="646bd-146">Его структура аналогична стандарту ISO/IEC 27002:2013.</span><span class="sxs-lookup"><span data-stu-id="646bd-146">It is structured in a format similar to ISO/IEC 27002:2013.</span></span>

<span data-ttu-id="646bd-147">**Где можно посмотреть сведения о соответствии требованиям Майкрософт ISO/IEC 27017:2015?**</span><span class="sxs-lookup"><span data-stu-id="646bd-147">**Where can I view Microsoft's compliance information for ISO/IEC 27017:2015?**</span></span>

<span data-ttu-id="646bd-148">Вы можете скачать [сертификат ISO/IEC 27017:2015](https://aka.ms/azureiso27017) для Azure, Intune и Power BI.</span><span class="sxs-lookup"><span data-stu-id="646bd-148">You can download the [ISO/IEC 27017:2015 certificate](https://aka.ms/azureiso27017) for Azure, Intune, and Power BI.</span></span>

<span data-ttu-id="646bd-149">**Можно ли использовать соответствие стандарту ISO/IEC 27017 для служб Майкрософт в процессе сертификации моей организации?**</span><span class="sxs-lookup"><span data-stu-id="646bd-149">**Can I use the ISO/IEC 27017 compliance of Microsoft services in my organization's certification process?**</span></span>

<span data-ttu-id="646bd-150">Да.</span><span class="sxs-lookup"><span data-stu-id="646bd-150">Yes.</span></span> <span data-ttu-id="646bd-151">Если ваша организации стремится пройти сертификацию для реализаций, развернутых в любых поддерживаемых корпоративных облачных службах Майкрософт, вы можете использовать соответствующие сертификаты Майкрософт при оценке соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="646bd-151">If your business is seeking certification for implementations deployed on any Microsoft in-scope enterprise cloud services, you can use Microsoft's relevant certifications in your compliance assessment.</span></span> <span data-ttu-id="646bd-152">Однако вы несете ответственность за привлечение аудитора для оценки реализации на соответствие требованиям, а также оценки средств управления и процессов в рамках вашей организации.</span><span class="sxs-lookup"><span data-stu-id="646bd-152">However, you are responsible for engaging an assessor to evaluate your implementation for compliance, and for the controls and processes within your own organization.</span></span>

<span data-ttu-id="646bd-153">**Как получить копии соответствующих отчетов об аудите?**</span><span class="sxs-lookup"><span data-stu-id="646bd-153">**How can I get copies of the applicable audit reports?**</span></span>

<span data-ttu-id="646bd-154">На портале [Service Trust Portal](https://aka.ms/stphelp) доступны отчеты о независимом аудите и другие сопутствующие документы.</span><span class="sxs-lookup"><span data-stu-id="646bd-154">The [Service Trust Portal](https://aka.ms/stphelp) provides independent, third-party audit reports and other related documentation.</span></span> <span data-ttu-id="646bd-155">Вы можете использовать этот портал для скачивания и просмотра этих документов, помогающих выполнять нормативные требования.</span><span class="sxs-lookup"><span data-stu-id="646bd-155">You can use the portal to download and review this documentation for assistance with your own regulatory requirements.</span></span>

## <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a><span data-ttu-id="646bd-156">Оценка риска с помощью диспетчера соответствия требованиям (Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="646bd-156">Use Microsoft Compliance Manager to assess your risk</span></span>

<span data-ttu-id="646bd-157">[Диспетчер соответствия требованиям (Майкрософт)](/microsoft-365/compliance/compliance-manager) — это предварительная функция в [Центре соответствия требованиям Microsoft 365](/microsoft-365/compliance/microsoft-365-compliance-center), помогающая понять состояние вашей организации в отношении соответствия требованиям и принять меры по снижению рисков.</span><span class="sxs-lookup"><span data-stu-id="646bd-157">[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft 365 compliance center](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks.</span></span> <span data-ttu-id="646bd-158">Диспетчер соответствия требованиям предоставляет премиум-шаблон для оценки этих нормативных требований.</span><span class="sxs-lookup"><span data-stu-id="646bd-158">Compliance Manager offers a premium template for building an assessment for this regulation.</span></span> <span data-ttu-id="646bd-159">Шаблон находится на странице **шаблонов оценки** в диспетчере соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="646bd-159">Find the template in the **assessment templates** page in Compliance Manager.</span></span> <span data-ttu-id="646bd-160">См. [Создание оценки в диспетчере соответствия требованиям](/microsoft-365/compliance/compliance-manager-assessments).</span><span class="sxs-lookup"><span data-stu-id="646bd-160">Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).</span></span>

## <a name="resources"></a><span data-ttu-id="646bd-161">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="646bd-161">Resources</span></span>

- [<span data-ttu-id="646bd-162">Свод правил ISO/IEC 27017:2015</span><span class="sxs-lookup"><span data-stu-id="646bd-162">ISO/IEC 27017:2015 code of practice</span></span>](https://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=43757)
- [<span data-ttu-id="646bd-163">Условия использования веб-служб Майкрософт</span><span class="sxs-lookup"><span data-stu-id="646bd-163">Microsoft Online Services Terms</span></span>](https://aka.ms/Online-Services-Terms)
- [<span data-ttu-id="646bd-164">Соответствие требованиям в центре управления безопасностью Майкрософт</span><span class="sxs-lookup"><span data-stu-id="646bd-164">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)
