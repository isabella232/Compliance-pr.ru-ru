---
title: Управление доступом к Microsoft 365 для мониторинга и аудита
description: Сводка. Сводка различных элементов управления доступом для мониторинга и аудита, доступных в Microsoft 365.
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
- MS-Compliance
f1.keywords:
- NOCSH
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: e9a9ea713afbf7568c1ae67d31a57dd9dce51fc3
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51497545"
---
# <a name="monitoring-and-auditing-access-controls-in-microsoft-365"></a><span data-ttu-id="8524c-103">Контроль и аудит элементов управления доступом в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8524c-103">Monitoring and auditing access controls in Microsoft 365</span></span>

<span data-ttu-id="8524c-104">Корпорация Майкрософт выполняет обширный мониторинг и аудит всех делегирования, привилегий и операций, которые происходят в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8524c-104">Microsoft performs extensive monitoring and auditing of all delegation, privileges, and operations that occur within Microsoft 365.</span></span> <span data-ttu-id="8524c-105">Управление доступом Microsoft 365 — это автоматизированный процесс, построенный по принципу наименьших привилегий и включающий элементы управления доступом к данным и аудита:</span><span class="sxs-lookup"><span data-stu-id="8524c-105">Microsoft 365 access control is an automated process built on the principle of least privilege and incorporating data access controls and audits:</span></span>

- <span data-ttu-id="8524c-106">Все разрешенные доступы отслеживаются для уникального пользователя.</span><span class="sxs-lookup"><span data-stu-id="8524c-106">All permitted access is traceable to a unique user.</span></span> <span data-ttu-id="8524c-107">Администраторы подотчетны за обработку контента клиента.</span><span class="sxs-lookup"><span data-stu-id="8524c-107">Administrators are accountable for their handling of customer content.</span></span>
- <span data-ttu-id="8524c-108">Запросы на управление доступом, журналы утверждений и административных операций захватываются для анализа безопасности и вредоносных событий.</span><span class="sxs-lookup"><span data-stu-id="8524c-108">Access control requests, approvals, and administrative operations logs are captured for analysis of security and malicious events.</span></span>
- <span data-ttu-id="8524c-109">Уровни доступа проверяются почти в режиме реального времени на основе членства в группе безопасности, чтобы обеспечить доступ к системам только пользователям, у которых есть авторизованные бизнес-обоснования и которые соответствуют требованиям, предъявляемым к требованиям.</span><span class="sxs-lookup"><span data-stu-id="8524c-109">Access levels are reviewed in near real-time based on security group membership to ensure that only users who have authorized business justifications and meet the eligibility requirements have access to the systems.</span></span>
- <span data-ttu-id="8524c-110">Microsoft 365, элементы управления доступом и вспомогательные службы, включая Azure Active Directory и физические центра обработки данных, регулярно проверяются независимыми сторонними сторонами на предмет соответствия требованиям [ISO/IEC 27001,](https://www.microsoft.com/TrustCenter/Compliance/iso-iec-27001) [ISO/IEC 27018,](https://www.microsoft.com/TrustCenter/Compliance/iso-iec-27018) [SOC,](https://www.microsoft.com/TrustCenter/Compliance/SOC) [FedRAMP (Office 365)](https://www.microsoft.com/TrustCenter/Compliance/FedRAMP)и другим стандартам [.](https://www.microsoft.com/TrustCenter/Compliance?service=Office#Icons)</span><span class="sxs-lookup"><span data-stu-id="8524c-110">Microsoft 365, its access controls, and supporting services, including Azure Active Directory and physical datacenters, are regularly audited by independent third-parties for compliance with [ISO/IEC 27001](https://www.microsoft.com/TrustCenter/Compliance/iso-iec-27001), [ISO/IEC 27018](https://www.microsoft.com/TrustCenter/Compliance/iso-iec-27018), [SOC](https://www.microsoft.com/TrustCenter/Compliance/SOC), [FedRAMP (Office 365)](https://www.microsoft.com/TrustCenter/Compliance/FedRAMP), and other [standards](https://www.microsoft.com/TrustCenter/Compliance?service=Office#Icons).</span></span>
- <span data-ttu-id="8524c-111">Инженеры Microsoft 365 должны ежегодно проходить обучение безопасности, пересматривать оптимальные процедуры повышенного доступа и признавать политики безопасности и конфиденциальности Корпорации Майкрософт для сохранения прав на службу.</span><span class="sxs-lookup"><span data-stu-id="8524c-111">Microsoft 365 engineers must take yearly security training, review elevated access best procedures, and acknowledge Microsoft's security and privacy policies to maintain entitlements to the service.</span></span>

<span data-ttu-id="8524c-112">Автоматические оповещения срабатывает при обнаружении подозрительной активности, например нескольких неудачных входах в течение короткого периода.</span><span class="sxs-lookup"><span data-stu-id="8524c-112">Automated alerts trigger when suspicious activity is detected, such as multiple failed logins within a short period.</span></span> <span data-ttu-id="8524c-113">Группа реагирования на безопасность Microsoft 365 использует машинное обучение и анализ больших данных для проверки и анализа действий, выявления нерегулярных схем доступа и активного реагирования на аномальную и незаконную деятельность.</span><span class="sxs-lookup"><span data-stu-id="8524c-113">The Microsoft 365 Security Response team uses machine learning and big data analysis to review and analyze activity, look for irregular access patterns, and proactively respond to anomalous and illicit activities.</span></span> <span data-ttu-id="8524c-114">Корпорация Майкрософт также использует специальную команду тестеров проникновения и участвует в периодических упражнениях Red Team и Blue Team для поиска проблем безопасности и контроля доступа в службе.</span><span class="sxs-lookup"><span data-stu-id="8524c-114">Microsoft also employs a dedicated team of penetration testers and engages in periodic Red Team and Blue Team exercises to find security and access control issues in the service.</span></span> <span data-ttu-id="8524c-115">Клиенты могут проверить эффективность систем управления доступом с помощью отчетов аудита и API управления, предоставляемых Корпорацией Майкрософт 365.</span><span class="sxs-lookup"><span data-stu-id="8524c-115">Customers can verify the effectiveness of access control systems by using audit reports and the management activity API provided by Microsoft 365.</span></span>

<span data-ttu-id="8524c-116">Дополнительные сведения см. в справке [об API API управления Office 365](/office/office-365-management-api/office-365-management-activity-api-reference) и аудите и отчетности [в Microsoft 365.](assurance-auditing-and-reporting-overview.md)</span><span class="sxs-lookup"><span data-stu-id="8524c-116">For more information, see [Office 365 Management Activity API reference](/office/office-365-management-api/office-365-management-activity-api-reference) and [Auditing and reporting in Microsoft 365](assurance-auditing-and-reporting-overview.md).</span></span>
