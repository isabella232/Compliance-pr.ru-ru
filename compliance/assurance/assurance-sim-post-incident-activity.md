---
title: 'Управление инцидентами безопасности Microsoft 365: действия после инцидента'
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
hideEdit: true
ms.openlocfilehash: 4ebd31c16f8abb3eddd6ed924a045d88597aba40
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51496713"
---
# <a name="microsoft-365-security-incident-management-post-incident-activity"></a><span data-ttu-id="100db-103">Управление инцидентами безопасности Microsoft 365: действия после инцидента</span><span class="sxs-lookup"><span data-stu-id="100db-103">Microsoft 365 security incident management: Post-incident activity</span></span>

## <a name="postmortem"></a><span data-ttu-id="100db-104">Postmortem</span><span class="sxs-lookup"><span data-stu-id="100db-104">Postmortem</span></span>

<span data-ttu-id="100db-105">Некоторые инциденты безопасности, особенно те инциденты, которые влияют на клиента или привели к нарушению данных, подвергаются полному инциденту посмертно.</span><span class="sxs-lookup"><span data-stu-id="100db-105">Some security incidents, especially those incidents that are customer impacting or result in a data breach, are subject to a full incident postmortem.</span></span> <span data-ttu-id="100db-106">Группа реагирования на безопасность Microsoft 365 проводит подробный посмертный отчет со всеми сторонами, участвующими в реагировании на инциденты безопасности:</span><span class="sxs-lookup"><span data-stu-id="100db-106">The Microsoft 365 Security Response team conducts a detailed postmortem with all the parties involved in security incident response to:</span></span>

- <span data-ttu-id="100db-107">Документировать последовательность событий, вызвавшего инцидент</span><span class="sxs-lookup"><span data-stu-id="100db-107">Document the sequence of events that caused the incident</span></span>
- <span data-ttu-id="100db-108">Создайте техническую сводку об инциденте, поддерживаемую доказательствами, которые включают участников нарушения (если они известны).</span><span class="sxs-lookup"><span data-stu-id="100db-108">Create a technical summary of the incident as supported by the evidence that includes the actors involved in the breach (if known).</span></span> <span data-ttu-id="100db-109">Это сводка будет включать в себя, как был выполнен ответ и другие ключевые выноски.</span><span class="sxs-lookup"><span data-stu-id="100db-109">This summary will include how the response was executed and other key takeaways.</span></span>
- <span data-ttu-id="100db-110">Определите технические ошибки, процедурные сбои, ошибки вручную, недостатки процесса и сбои связи и/или какие-либо ранее неизвестные векторы атак, которые были идентифицированы во время реагирования на инциденты безопасности.</span><span class="sxs-lookup"><span data-stu-id="100db-110">Identify technical lapses, procedural failures, manual errors, process flaws, and communication glitches, and/or any previously unknown attack vectors that were identified during the security incident response.</span></span>

<span data-ttu-id="100db-111">Посмертный процесс непосредственно повлияет на улучшение службы Microsoft 365, операционные процессы и документацию, установив новые приоритеты в цикле разработки инженерной разработки Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="100db-111">The postmortem will directly influence Microsoft 365 service improvement, operational processes, and documentation by setting new priorities in the Microsoft 365 engineering development cycle.</span></span>

## <a name="documentation"></a><span data-ttu-id="100db-112">Документация</span><span class="sxs-lookup"><span data-stu-id="100db-112">Documentation</span></span>

<span data-ttu-id="100db-113">Все ключевые технические результаты посмертного процесса запечатлены в отчете и инвестициях в службу или исправлении в виде ошибок или запросов на изменение разработки.</span><span class="sxs-lookup"><span data-stu-id="100db-113">All key technical findings in the postmortem process are captured in a report and service investments or fixes in the form of bugs or development change requests.</span></span> <span data-ttu-id="100db-114">Эти выводы следует за соответствующими группами инженеров.</span><span class="sxs-lookup"><span data-stu-id="100db-114">These findings are followed-up with the appropriate engineering teams.</span></span> <span data-ttu-id="100db-115">При сбоях процессов и проблемах, которые могут быть перекрестными, проблемы задокументированы в базе данных группы реагирования на безопасность Microsoft 365 и следуют за соответствующими группами для их устранения.</span><span class="sxs-lookup"><span data-stu-id="100db-115">For process failures and cross-organizational issues, issues are documented in the Microsoft 365 Security Response team's database and followed-up with the appropriate groups to address them.</span></span>

## <a name="process-improvement"></a><span data-ttu-id="100db-116">Улучшение процессов</span><span class="sxs-lookup"><span data-stu-id="100db-116">Process improvement</span></span>

<span data-ttu-id="100db-117">Реагирование на инцидент с безопасностью в Microsoft 365 предполагает координацию с несколькими группами, распространяющихся по различным организациям в Корпорации Майкрософт, и потенциально даже с соответствующими внешними организациями, такими как правоохранительные органы.</span><span class="sxs-lookup"><span data-stu-id="100db-117">Responding to a security incident in Microsoft 365 involves coordination with multiple groups spread across different organizations within Microsoft, and potentially even appropriate external organizations such as law enforcement.</span></span> <span data-ttu-id="100db-118">Мы знаем, что очень важно оценить наши ответы после каждого инцидента с безопасностью как для достаточности, так и для полноты.</span><span class="sxs-lookup"><span data-stu-id="100db-118">We know that it is critical to evaluate our responses after every security incident for both sufficiency and completeness.</span></span> <span data-ttu-id="100db-119">Для любых выявленных улучшений или изменений группа реагирования на безопасность Microsoft 365 оценивает предложения в консультации с соответствующими группами и заинтересованными сторонами и, где это необходимо, включает их в стандартные операционные процедуры.</span><span class="sxs-lookup"><span data-stu-id="100db-119">For any identified improvements or changes, the Microsoft 365 Security Response team evaluates the suggestions in consultation with the appropriate teams and stakeholders, and where appropriate incorporates them into standard operating procedures.</span></span> <span data-ttu-id="100db-120">Все необходимые изменения, ошибки или улучшения службы, выявленные во время реагирования на инциденты безопасности или посмертной активности, регистрируются и отслеживаются во внутренней инженерной базе данных Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="100db-120">All required changes, bugs, or service improvements identified during the security incident response or postmortem activity are logged and tracked in an internal Microsoft 365 engineering database.</span></span> <span data-ttu-id="100db-121">Все потенциальные ошибки или функции назначены соответствующему владельцу.</span><span class="sxs-lookup"><span data-stu-id="100db-121">All potential bugs or features are assigned to the appropriate owner.</span></span> <span data-ttu-id="100db-122">Группа реагирования на безопасность Microsoft 365 проверяет все записи до тех пор, пока проблема не будет устранена.</span><span class="sxs-lookup"><span data-stu-id="100db-122">The Microsoft 365 Security Response team reviews all entries until the issue is resolved.</span></span>

## <a name="related-articles"></a><span data-ttu-id="100db-123">Статьи по теме</span><span class="sxs-lookup"><span data-stu-id="100db-123">Related articles</span></span>

- [<span data-ttu-id="100db-124">Управление инцидентами, связанными с безопасностью, в Microsoft 365 </span><span class="sxs-lookup"><span data-stu-id="100db-124">Microsoft 365 security incident management</span></span>](assurance-security-incident-management.md)
- [<span data-ttu-id="100db-125">Подготовка к управлению инцидентами безопасности Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="100db-125">Microsoft 365 security incident management preparation</span></span>](assurance-sim-preparation.md)
- [<span data-ttu-id="100db-126">Обнаружение и анализ инцидентов безопасности Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="100db-126">Microsoft 365 security incident management detection and analysis</span></span>](assurance-sim-detection-analysis.md)
- [<span data-ttu-id="100db-127">Сдерживание, ликвидация и восстановление инцидентов безопасности Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="100db-127">Microsoft 365 security incident management containment, eradication, and recovery</span></span>](assurance-sim-containment-eradication-recovery.md)
