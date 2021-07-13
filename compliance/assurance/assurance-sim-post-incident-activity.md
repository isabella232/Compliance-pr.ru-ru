---
title: 'Управление инцидентами безопасности Майкрософт: действие после инцидента'
description: В этой статье представлен обзор процесса управления инцидентами безопасности после инцидента в онлайн-службах Microsoft.
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
hideEdit: true
ms.openlocfilehash: 965c7d6d0d469b9eea981252805bda598c92a4c8
ms.sourcegitcommit: 8bf2602d56eedee4447ddb374ef95b0587f254e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2021
ms.locfileid: "53377536"
---
# <a name="microsoft-security-incident-management-post-incident-activity"></a><span data-ttu-id="aa038-103">Управление инцидентами безопасности Майкрософт: действие после инцидента</span><span class="sxs-lookup"><span data-stu-id="aa038-103">Microsoft security incident management: Post-incident activity</span></span>

## <a name="postmortem"></a><span data-ttu-id="aa038-104">Postmortem</span><span class="sxs-lookup"><span data-stu-id="aa038-104">Postmortem</span></span>

<span data-ttu-id="aa038-105">Некоторые инциденты безопасности, особенно те инциденты, которые влияют на клиента или привели к нарушению данных, подвергаются полному инциденту посмертно.</span><span class="sxs-lookup"><span data-stu-id="aa038-105">Some security incidents, especially those incidents that are customer impacting or result in a data breach, are subject to a full incident postmortem.</span></span> <span data-ttu-id="aa038-106">Группа реагирования на безопасность проводит подробный посмертный отчет со всеми сторонами, участвующими в реагировании на инциденты безопасности:</span><span class="sxs-lookup"><span data-stu-id="aa038-106">The security response team conducts a detailed postmortem with all the parties involved in security incident response to:</span></span>

- <span data-ttu-id="aa038-107">Документировать последовательность событий, вызвавшего инцидент.</span><span class="sxs-lookup"><span data-stu-id="aa038-107">Document the sequence of events that caused the incident.</span></span>
- <span data-ttu-id="aa038-108">Создайте техническую сводку об инциденте, поддерживаемую доказательствами, которые включают участников нарушения (если они известны).</span><span class="sxs-lookup"><span data-stu-id="aa038-108">Create a technical summary of the incident as supported by the evidence that includes the actors involved in the breach (if known).</span></span> <span data-ttu-id="aa038-109">Это сводка будет включать в себя, как был выполнен ответ и другие ключевые выноски.</span><span class="sxs-lookup"><span data-stu-id="aa038-109">This summary will include how the response was executed and other key takeaways.</span></span>
- <span data-ttu-id="aa038-110">Определите технические ошибки, процедурные сбои, ошибки вручную, недостатки процесса и сбои связи и/или какие-либо ранее неизвестные векторы атак, которые были идентифицированы во время реагирования на инциденты безопасности.</span><span class="sxs-lookup"><span data-stu-id="aa038-110">Identify technical lapses, procedural failures, manual errors, process flaws, and communication glitches, and/or any previously unknown attack vectors that were identified during the security incident response.</span></span>

<span data-ttu-id="aa038-111">Посмертный процесс непосредственно влияет на совершенствование служб Майкрософт в Интернете, операционные процессы и документацию, устанавливая новые приоритеты в цикле разработки инженерных служб Microsoft online.</span><span class="sxs-lookup"><span data-stu-id="aa038-111">The postmortem will directly influence Microsoft online service improvement, operational processes, and documentation by setting new priorities in the Microsoft online services engineering development cycle.</span></span>

## <a name="documentation"></a><span data-ttu-id="aa038-112">Документация</span><span class="sxs-lookup"><span data-stu-id="aa038-112">Documentation</span></span>

<span data-ttu-id="aa038-113">Все ключевые технические результаты посмертного процесса запечатлены в отчете и инвестициях в службу или исправлении в виде ошибок или запросов на изменение разработки.</span><span class="sxs-lookup"><span data-stu-id="aa038-113">All key technical findings in the postmortem process are captured in a report and service investments or fixes in the form of bugs or development change requests.</span></span> <span data-ttu-id="aa038-114">Эти выводы следует за соответствующими группами инженеров.</span><span class="sxs-lookup"><span data-stu-id="aa038-114">These findings are followed-up with the appropriate engineering teams.</span></span> <span data-ttu-id="aa038-115">При сбоях процессов и меж организационных проблемах проблемы задокументированы в базе данных группы реагирования на безопасность и последует за соответствующими группами для их устранения.</span><span class="sxs-lookup"><span data-stu-id="aa038-115">For process failures and cross-organizational issues, issues are documented in the security response team's database and followed-up with the appropriate groups to address them.</span></span>

## <a name="process-improvement"></a><span data-ttu-id="aa038-116">Улучшение процессов</span><span class="sxs-lookup"><span data-stu-id="aa038-116">Process improvement</span></span>

<span data-ttu-id="aa038-117">Реагирование на инцидент с безопасностью в онлайн-службах Microsoft включает координацию с несколькими группами, распространяющихся по различным организациям в Корпорации Майкрософт, и потенциально даже соответствующими внешними организациями, такими как правоохранительные органы.</span><span class="sxs-lookup"><span data-stu-id="aa038-117">Responding to a security incident in Microsoft online services involves coordination with multiple groups spread across different organizations within Microsoft, and potentially even appropriate external organizations such as law enforcement.</span></span> <span data-ttu-id="aa038-118">Мы знаем, что очень важно оценить наши ответы после каждого инцидента с безопасностью как для достаточности, так и для полноты.</span><span class="sxs-lookup"><span data-stu-id="aa038-118">We know that it is critical to evaluate our responses after every security incident for both sufficiency and completeness.</span></span> <span data-ttu-id="aa038-119">При любых выявленных улучшениях или изменениях группа реагирования на безопасность оценивает предложения в консультации с соответствующими группами и заинтересованными сторонами и при необходимости включает их в стандартные операционные процедуры.</span><span class="sxs-lookup"><span data-stu-id="aa038-119">For any identified improvements or changes, the security response team evaluates the suggestions in consultation with the appropriate teams and stakeholders, and where appropriate incorporates them into standard operating procedures.</span></span> <span data-ttu-id="aa038-120">Все необходимые изменения, ошибки или улучшения службы, выявленные во время реагирования на инциденты безопасности или посмертной активности, регистрируются и отслеживаются во внутренней базе данных инженерии Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="aa038-120">All required changes, bugs, or service improvements identified during the security incident response or postmortem activity are logged and tracked in an internal Microsoft engineering database.</span></span> <span data-ttu-id="aa038-121">Все потенциальные ошибки или функции назначены соответствующему владельцу.</span><span class="sxs-lookup"><span data-stu-id="aa038-121">All potential bugs or features are assigned to the appropriate owner.</span></span> <span data-ttu-id="aa038-122">Группа реагирования на безопасность Майкрософт проверяет все записи до тех пор, пока проблема не будет устранена.</span><span class="sxs-lookup"><span data-stu-id="aa038-122">The Microsoft security response team reviews all entries until the issue is resolved.</span></span>

## <a name="related-articles"></a><span data-ttu-id="aa038-123">Статьи по теме</span><span class="sxs-lookup"><span data-stu-id="aa038-123">Related articles</span></span>

- [<span data-ttu-id="aa038-124">Управление инцидентами безопасности Майкрософт</span><span class="sxs-lookup"><span data-stu-id="aa038-124">Microsoft security incident management</span></span>](assurance-security-incident-management.md)
- [<span data-ttu-id="aa038-125">Управление инцидентами безопасности Майкрософт: подготовка</span><span class="sxs-lookup"><span data-stu-id="aa038-125">Microsoft security incident management: Preparation</span></span>](assurance-sim-preparation.md)
- [<span data-ttu-id="aa038-126">Управление инцидентами безопасности Майкрософт: обнаружение и анализ</span><span class="sxs-lookup"><span data-stu-id="aa038-126">Microsoft security incident management: Detection and analysis</span></span>](assurance-sim-detection-analysis.md)
- [<span data-ttu-id="aa038-127">Управление инцидентами безопасности Майкрософт: сдерживание, ликвидация и восстановление</span><span class="sxs-lookup"><span data-stu-id="aa038-127">Microsoft security incident management: Containment, eradication, and recovery</span></span>](assurance-sim-containment-eradication-recovery.md)
- [<span data-ttu-id="aa038-128">Как войти в журнал билета поддержки событий безопасности</span><span class="sxs-lookup"><span data-stu-id="aa038-128">How to Log a Security Event Support Ticket</span></span>](/azure/security/fundamentals/event-support-ticket)
- [<span data-ttu-id="aa038-129">Azure и Dynamics 365: уведомление о нарушении безопасности данных согласно GDPR</span><span class="sxs-lookup"><span data-stu-id="aa038-129">Azure and Dynamics 365 breach notification under the GDPR</span></span>](/compliance/regulatory/gdpr-breach-azure-dynamics)
