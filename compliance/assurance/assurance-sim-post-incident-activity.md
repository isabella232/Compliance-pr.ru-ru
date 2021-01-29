---
title: 'Управление инцидентами безопасности в Microsoft 365: действия после инцидента'
description: В этой статье представлен обзор процесса управления инцидентами безопасности после инцидента в Microsoft 365.
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
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: 66c25503ac574de512f5201981112a0e54714968
ms.sourcegitcommit: 2973d25e9e0185b84d281f963553a332eac1c1a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50040352"
---
# <a name="microsoft-365-security-incident-management-post-incident-activity"></a><span data-ttu-id="2be06-103">Управление инцидентами безопасности в Microsoft 365: действия после инцидента</span><span class="sxs-lookup"><span data-stu-id="2be06-103">Microsoft 365 security incident management: Post-incident activity</span></span>

## <a name="postmortem"></a><span data-ttu-id="2be06-104">Postmortem</span><span class="sxs-lookup"><span data-stu-id="2be06-104">Postmortem</span></span>

<span data-ttu-id="2be06-105">Некоторые инциденты безопасности, особенно инциденты, которые влияют на клиентов или могут привести к нарушению безопасности данных, подвержены полному нарушению после инцидента.</span><span class="sxs-lookup"><span data-stu-id="2be06-105">Some security incidents, especially those incidents that are customer impacting or result in a data breach, are subject to a full incident postmortem.</span></span> <span data-ttu-id="2be06-106">Группа реагирования на инциденты безопасности Microsoft 365 проводит подробный анализ со всеми сторонами, участвующими в реагировании на инциденты безопасности, для:</span><span class="sxs-lookup"><span data-stu-id="2be06-106">The Microsoft 365 Security Response team conducts a detailed postmortem with all the parties involved in security incident response to:</span></span>

- <span data-ttu-id="2be06-107">Документировать последовательность событий, вызвавшего инцидент</span><span class="sxs-lookup"><span data-stu-id="2be06-107">Document the sequence of events that caused the incident</span></span>
- <span data-ttu-id="2be06-108">Создайте техническую сводку по инциденту, поддерживаемую свидетельством, которое включает субъектов, участвующих в нарушении (если известно).</span><span class="sxs-lookup"><span data-stu-id="2be06-108">Create a technical summary of the incident as supported by the evidence that includes the actors involved in the breach (if known).</span></span> <span data-ttu-id="2be06-109">Эта сводка содержит сведения о том, как был выполнен ответ, и другие важные сведения.</span><span class="sxs-lookup"><span data-stu-id="2be06-109">This summary will include how the response was executed and other key takeaways.</span></span>
- <span data-ttu-id="2be06-110">Определите технические ошибки, процедурные сбои, ошибки вручную, недостатки процесса и сбои связи, а также/или любые ранее неизвестные векторы атаки, выявленные во время реагирования на инциденты безопасности.</span><span class="sxs-lookup"><span data-stu-id="2be06-110">Identify technical lapses, procedural failures, manual errors, process flaws, and communication glitches, and/or any previously unknown attack vectors that were identified during the security incident response.</span></span>

<span data-ttu-id="2be06-111">Послеморем напрямую повлияет на улучшение службы Microsoft 365, операционные процессы и документацию, установив новые приоритеты в цикле разработки microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2be06-111">The postmortem will directly influence Microsoft 365 service improvement, operational processes, and documentation by setting new priorities in the Microsoft 365 engineering development cycle.</span></span>

## <a name="documentation"></a><span data-ttu-id="2be06-112">Документация</span><span class="sxs-lookup"><span data-stu-id="2be06-112">Documentation</span></span>

<span data-ttu-id="2be06-113">Все ключевые технические выводы в процессе postmortem фиксироваться в отчете и инвестициях в службы или исправлениях в виде ошибок или запросов на изменение разработки.</span><span class="sxs-lookup"><span data-stu-id="2be06-113">All key technical findings in the postmortem process are captured in a report and service investments or fixes in the form of bugs or development change requests.</span></span> <span data-ttu-id="2be06-114">На эти выводы следят соответствующие инженерные группы.</span><span class="sxs-lookup"><span data-stu-id="2be06-114">These findings are followed-up with the appropriate engineering teams.</span></span> <span data-ttu-id="2be06-115">При сбоях процессов и межуправленных проблемах проблемы задокументированы в базе данных группы реагирования на угрозы безопасности Microsoft 365 и следуют за соответствующими группами для их решения.</span><span class="sxs-lookup"><span data-stu-id="2be06-115">For process failures and cross-organizational issues, issues are documented in the Microsoft 365 Security Response team's database and followed-up with the appropriate groups to address them.</span></span>

## <a name="process-improvement"></a><span data-ttu-id="2be06-116">Улучшение процессов</span><span class="sxs-lookup"><span data-stu-id="2be06-116">Process improvement</span></span>

<span data-ttu-id="2be06-117">Реагирование на инцидент безопасности в Microsoft 365 включает координацию с несколькими группами, которые распространяются в различных организациях Майкрософт и, возможно, даже в соответствующих внешних организациях, таких как правоохранительные органы.</span><span class="sxs-lookup"><span data-stu-id="2be06-117">Responding to a security incident in Microsoft 365 involves coordination with multiple groups spread across different organizations within Microsoft, and potentially even appropriate external organizations such as law enforcement.</span></span> <span data-ttu-id="2be06-118">Мы знаем, что очень важно оценить наши ответы после каждого инцидента безопасности как на статическую, так и на полную.</span><span class="sxs-lookup"><span data-stu-id="2be06-118">We know that it is critical to evaluate our responses after every security incident for both sufficiency and completeness.</span></span> <span data-ttu-id="2be06-119">В случае любых выявленных улучшений или изменений группа реагирования на угрозы безопасности Microsoft 365 оценивает предложения в консультации с соответствующими группами и заинтересованными сторонами и, где это необходимо, включает их в стандартные операционные процедуры.</span><span class="sxs-lookup"><span data-stu-id="2be06-119">For any identified improvements or changes, the Microsoft 365 Security Response team evaluates the suggestions in consultation with the appropriate teams and stakeholders, and where appropriate incorporates them into standard operating procedures.</span></span> <span data-ttu-id="2be06-120">Все необходимые изменения, ошибки или улучшения служб, выявленные во время реагирования на инциденты безопасности или действия после заморозки, регистрируются и отслеживаются во внутренней базе данных разработки Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2be06-120">All required changes, bugs, or service improvements identified during the security incident response or postmortem activity are logged and tracked in an internal Microsoft 365 engineering database.</span></span> <span data-ttu-id="2be06-121">Все потенциальные ошибки или функции назначены соответствующему владельцу.</span><span class="sxs-lookup"><span data-stu-id="2be06-121">All potential bugs or features are assigned to the appropriate owner.</span></span> <span data-ttu-id="2be06-122">Группа реагирования на угрозы безопасности Microsoft 365 проверяет все записи, пока проблема не будет устранена.</span><span class="sxs-lookup"><span data-stu-id="2be06-122">The Microsoft 365 Security Response team reviews all entries until the issue is resolved.</span></span>

## <a name="related-articles"></a><span data-ttu-id="2be06-123">Статьи по теме</span><span class="sxs-lookup"><span data-stu-id="2be06-123">Related articles</span></span>

- [<span data-ttu-id="2be06-124">Управление инцидентами безопасности в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2be06-124">Microsoft 365 security incident management</span></span>](assurance-security-incident-management.md)
- [<span data-ttu-id="2be06-125">Подготовка к управлению инцидентами безопасности Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2be06-125">Microsoft 365 security incident management preparation</span></span>](assurance-sim-preparation.md)
- [<span data-ttu-id="2be06-126">Обнаружение и анализ инцидентов безопасности Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2be06-126">Microsoft 365 security incident management detection and analysis</span></span>](assurance-sim-detection-analysis.md)
- [<span data-ttu-id="2be06-127">Управление инцидентами безопасности, уничтожение и восстановление Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2be06-127">Microsoft 365 security incident management containment, eradication, and recovery</span></span>](assurance-sim-containment-eradication-recovery.md)
