---
title: Рекомендации по специальным возможностям для веб-контента
description: Майкрософт публикует отчеты WCAG AA, целиком описывающие продукт, службу или части продукта, которые можно установить отдельно.
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
ms.openlocfilehash: 6330ee298949353c24a4b95ff65696807b78b09b
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53088798"
---
# <a name="web-content-accessibility-guidelines"></a><span data-ttu-id="a0642-104">Рекомендации по специальным возможностям для веб-контента</span><span class="sxs-lookup"><span data-stu-id="a0642-104">Web Content Accessibility Guidelines</span></span>

## <a name="about-wcag"></a><span data-ttu-id="a0642-105">Сведения о WCAG</span><span class="sxs-lookup"><span data-stu-id="a0642-105">About WCAG</span></span>

<span data-ttu-id="a0642-106">Рекомендации по специальным возможностям для веб-контента (WCAG) обеспечивают основу для повышения доступности веб-контента для людей с ограниченными возможностями.</span><span class="sxs-lookup"><span data-stu-id="a0642-106">The Web Content Accessibility Guidelines (WCAG) provide a framework for making web content more accessible for people with disabilities.</span></span> <span data-ttu-id="a0642-107">Рекомендации WCAG версии 2.0 были опубликованы в 2008 г. консорциумом W3C, международной организацией, занимающейся созданием веб-стандартов. Они были обновлены до WCAG 2.1 в июне 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a0642-107">WCAG version 2.0 was published in 2008 by the World Wide Web Consortium (W3C), an international organization dedicated to creating web standards, and updated to WCAG 2.1 in June 2018.</span></span> <span data-ttu-id="a0642-108">В 2012 г. руководство WCAG 2.0 также было опубликовано Международной организацией по стандартизации (ISO) в виде стандарта ISO/IEC 40500:2012.</span><span class="sxs-lookup"><span data-stu-id="a0642-108">In 2012, WCAG 2.0 was also published by the International Organization for Standardization (ISO) as ISO/IEC 40500:2012.</span></span>

<span data-ttu-id="a0642-109">Контент, соответствующий WCAG 2.1, также соответствует WCAG 2.0.</span><span class="sxs-lookup"><span data-stu-id="a0642-109">Content that conforms to WCAG 2.1 also conforms to WCAG 2.0.</span></span> <span data-ttu-id="a0642-110">Для политик, которые должны соответствовать WCAG 2.0, в руководстве WCAG 2.1 могут содержаться альтернативные способы обеспечения соответствия.</span><span class="sxs-lookup"><span data-stu-id="a0642-110">For policies requiring conformance to WCAG 2.0, WCAG 2.1 can provide an alternate means of conformance.</span></span>

<span data-ttu-id="a0642-111">Корпорация Майкрософт является основным поставщиком программного обеспечения и облачных служб для потребителей, предприятий и правительственных организаций по всему миру.</span><span class="sxs-lookup"><span data-stu-id="a0642-111">Microsoft is a major software and cloud-services provider to consumers, businesses, and governments around the world.</span></span> <span data-ttu-id="a0642-112">Чтобы помочь клиентам принимать решения о покупке, Майкрософт публикует отчеты о соответствии специальных возможностей, в которых описывается степень соответствия наших продуктов и служб стандарту WCAG.</span><span class="sxs-lookup"><span data-stu-id="a0642-112">To assist customers in making purchasing decisions, Microsoft publishes Accessibility Conformance Reports describing the extent to which our products and services support the WCAG criteria.</span></span> <span data-ttu-id="a0642-113">Эти сведения могут помочь клиентам Майкрософт определить, соответствует ли определенный продукт или служба их конкретным требованиям.</span><span class="sxs-lookup"><span data-stu-id="a0642-113">This information can help Microsoft customers determine whether a particular product or service will meet their specific needs.</span></span>
  
## <a name="microsoft-and-wcag"></a><span data-ttu-id="a0642-114">Майкрософт и WCAG</span><span class="sxs-lookup"><span data-stu-id="a0642-114">Microsoft and WCAG</span></span>

<span data-ttu-id="a0642-115">Майкрософт учитывает стандарт WCAG при разработке продуктов и служб, стремясь обеспечить доступность технологий и данных для всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="a0642-115">Microsoft's consideration of the WCAG standard in the development of products and services points to its commitment to making technology and data accessible for all customers.</span></span>

<span data-ttu-id="a0642-116">Майкрософт публикует отчеты WCAG, содержащие полное описание продукта или службы.</span><span class="sxs-lookup"><span data-stu-id="a0642-116">Microsoft publishes WCAG reports that reflect the complete product or service.</span></span> <span data-ttu-id="a0642-117">Как правило, отчеты для отдельных функций или компонентов не создаются.</span><span class="sxs-lookup"><span data-stu-id="a0642-117">It generally does not create reports for individual features or components.</span></span> <span data-ttu-id="a0642-118">Иногда корпорация Майкрософт может выпустить новый компонент для существующего продукта или новую версию существующего компонента, который пользователи могут устанавливать отдельно. Майкрософт может опубликовать отчет WCAG для такого компонента.</span><span class="sxs-lookup"><span data-stu-id="a0642-118">Sometimes, Microsoft might release a new component for an existing product, or a new version of an existing component, which users can choose to install separately, and Microsoft might also publish a WCAG report for that component.</span></span>

[<span data-ttu-id="a0642-119">Скачать стандарты специальных возможностей WCAG (ISO/IEC 40500)</span><span class="sxs-lookup"><span data-stu-id="a0642-119">Download the WCAG (ISO/IEC 40500) accessibility standards</span></span>](https://www.w3.org/WAI/standards-guidelines/wcag/)

## <a name="microsoft-in-scope-cloud-services"></a><span data-ttu-id="a0642-120">Облачные службы Майкрософт, к которым применима оценка</span><span class="sxs-lookup"><span data-stu-id="a0642-120">Microsoft in-scope cloud services</span></span>

- [<span data-ttu-id="a0642-121">Azure и Azure для государственных организаций</span><span class="sxs-lookup"><span data-stu-id="a0642-121">Azure and Azure Government</span></span>](https://go.microsoft.com/fwlink/p/?linkid=2051569)
- <span data-ttu-id="a0642-122">Azure DevOps Services</span><span class="sxs-lookup"><span data-stu-id="a0642-122">Azure DevOps Services</span></span>
- <span data-ttu-id="a0642-123">Dynamics 365 и Dynamics 365 для государственных организаций США</span><span class="sxs-lookup"><span data-stu-id="a0642-123">Dynamics 365 and Dynamics 365 U.S. Government</span></span>
- <span data-ttu-id="a0642-124">Intune</span><span class="sxs-lookup"><span data-stu-id="a0642-124">Intune</span></span>
- <span data-ttu-id="a0642-125">Office 365 и Office 365 для государственных организаций США</span><span class="sxs-lookup"><span data-stu-id="a0642-125">Office 365 and Office 365 U.S. Government</span></span>
- <span data-ttu-id="a0642-126">Office 365 для министерства обороны США</span><span class="sxs-lookup"><span data-stu-id="a0642-126">Office 365 U.S. Government Defense</span></span>
- <span data-ttu-id="a0642-127">Windows Server 2016</span><span class="sxs-lookup"><span data-stu-id="a0642-127">Windows Server 2016</span></span>

## <a name="microsoft-accessibility-conformance-reports"></a><span data-ttu-id="a0642-128">Отчеты Майкрософт по обеспечению доступности</span><span class="sxs-lookup"><span data-stu-id="a0642-128">Microsoft accessibility conformance reports</span></span>

<span data-ttu-id="a0642-129">Ознакомьтесь с отчетами WCAG для [всех наших продуктов и служб](https://cloudblogs.microsoft.com/industry-blog/government/2018/09/11/accessibility-conformance-reports/).</span><span class="sxs-lookup"><span data-stu-id="a0642-129">Read WCAG reports for [all our products and services](https://cloudblogs.microsoft.com/industry-blog/government/2018/09/11/accessibility-conformance-reports/).</span></span>

## <a name="resources"></a><span data-ttu-id="a0642-130">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="a0642-130">Resources</span></span>

- <span data-ttu-id="a0642-131">[Сайт о специальных возможностях Майкрософт](https://www.microsoft.com/accessibility): ознакомьтесь с использованием функций специальных возможностей и изучите, как инновации корпорации Майкрософт помогают каждому достичь большего.</span><span class="sxs-lookup"><span data-stu-id="a0642-131">[Microsoft accessibility site](https://www.microsoft.com/accessibility): Get information on using accessibility features and explore the ways Microsoft innovates to help everyone achieve more.</span></span>
- <span data-ttu-id="a0642-132">[Центр специальных возможностей Office 365](https://go.microsoft.com/fwlink/p/?linkid=2051801). Ресурсы Office 365 для людей с ограниченными возможностями.</span><span class="sxs-lookup"><span data-stu-id="a0642-132">[Office 365 Accessibility Center](https://go.microsoft.com/fwlink/p/?linkid=2051801): Office 365 resources for people with disabilities.</span></span>
- <span data-ttu-id="a0642-133">[Enterprise Disability Answer Desk](https://go.microsoft.com/fwlink/p/?linkid=2050890). Поддержка для корпоративных клиентов с вопросами о специальных возможностях наших продуктов и служб или о соответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="a0642-133">[Enterprise Disability Answer Desk](https://go.microsoft.com/fwlink/p/?linkid=2050890): Dedicated support for enterprise customers with accessibility questions about our products and services or compliance.</span></span>
- [<span data-ttu-id="a0642-134">Соответствие требованиям в центре управления безопасностью Майкрософт</span><span class="sxs-lookup"><span data-stu-id="a0642-134">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)
