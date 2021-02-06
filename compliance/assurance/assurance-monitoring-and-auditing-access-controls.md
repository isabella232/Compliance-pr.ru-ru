---
title: Средства контроля доступа для мониторинга и аудита Microsoft 365
description: Сводка. Сводка по различным средствам мониторинга и аудита доступа, доступным в Microsoft 365.
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
ms.openlocfilehash: 3021ce1dd59d5d071edec22286ae9c63833f1277
ms.sourcegitcommit: 21ed42335efd37774ff5d17d9586d5546147241a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2021
ms.locfileid: "50120448"
---
# <a name="monitoring-and-auditing-access-controls-in-microsoft-365"></a><span data-ttu-id="228be-103">Мониторинг и аудит элементов управления доступом в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="228be-103">Monitoring and auditing access controls in Microsoft 365</span></span>

<span data-ttu-id="228be-104">Корпорация Майкрософт выполняет обширный мониторинг и аудит всех делегирования, привилегий и операций, которые выполняются в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="228be-104">Microsoft performs extensive monitoring and auditing of all delegation, privileges, and operations that occur within Microsoft 365.</span></span> <span data-ttu-id="228be-105">Управление доступом Microsoft 365 — это автоматизированный процесс, построенный на принципе наименьших привилегий и включающий в себя элементы управления доступом к данным и аудиты:</span><span class="sxs-lookup"><span data-stu-id="228be-105">Microsoft 365 access control is an automated process built on the principle of least privilege and incorporating data access controls and audits:</span></span>

- <span data-ttu-id="228be-106">Весь разрешенный доступ можно отследить для уникального пользователя.</span><span class="sxs-lookup"><span data-stu-id="228be-106">All permitted access is traceable to a unique user.</span></span> <span data-ttu-id="228be-107">Администраторы имеют ответственность за обработку контента клиентов.</span><span class="sxs-lookup"><span data-stu-id="228be-107">Administrators are accountable for their handling of customer content.</span></span>
- <span data-ttu-id="228be-108">Запросы управления доступом, утверждения и журналы административных операций регистрются для анализа событий безопасности и вредоносных событий.</span><span class="sxs-lookup"><span data-stu-id="228be-108">Access control requests, approvals, and administrative operations logs are captured for analysis of security and malicious events.</span></span>
- <span data-ttu-id="228be-109">Уровни доступа проверяются практически в режиме реального времени на основе членства в группах безопасности, чтобы обеспечить доступ к системам только тем пользователям, у которых есть авторизованные бизнес-обоснования и которые соответствуют требованиям.</span><span class="sxs-lookup"><span data-stu-id="228be-109">Access levels are reviewed in near real-time based on security group membership to ensure that only users who have authorized business justifications and meet the eligibility requirements have access to the systems.</span></span>
- <span data-ttu-id="228be-110">Microsoft 365, его средства контроля доступа и вспомогательные службы, включая Azure Active Directory и физические центра обработки данных, регулярно проверяются независимыми сторонними лицами на соответствие требованиям [ISO/IEC 27001,](https://www.microsoft.com/TrustCenter/Compliance/iso-iec-27001) [ISO/IEC 27018,](https://www.microsoft.com/TrustCenter/Compliance/iso-iec-27018) [SOC,](https://www.microsoft.com/TrustCenter/Compliance/SOC) [FedRAMP (Office 365)](https://www.microsoft.com/TrustCenter/Compliance/FedRAMP)и другим [стандартам.](https://www.microsoft.com/TrustCenter/Compliance?service=Office#Icons)</span><span class="sxs-lookup"><span data-stu-id="228be-110">Microsoft 365, its access controls, and supporting services, including Azure Active Directory and physical datacenters, are regularly audited by independent third-parties for compliance with [ISO/IEC 27001](https://www.microsoft.com/TrustCenter/Compliance/iso-iec-27001), [ISO/IEC 27018](https://www.microsoft.com/TrustCenter/Compliance/iso-iec-27018), [SOC](https://www.microsoft.com/TrustCenter/Compliance/SOC), [FedRAMP (Office 365)](https://www.microsoft.com/TrustCenter/Compliance/FedRAMP), and other [standards](https://www.microsoft.com/TrustCenter/Compliance?service=Office#Icons).</span></span>
- <span data-ttu-id="228be-111">Инженеры Microsoft 365 должны ежегодно проходить обучение безопасности, пересматривать лучшие процедуры доступа с повышенными правами и подтверждать политики безопасности и конфиденциальности Корпорации Майкрософт для обслуживания прав на службу.</span><span class="sxs-lookup"><span data-stu-id="228be-111">Microsoft 365 engineers must take yearly security training, review elevated access best procedures, and acknowledge Microsoft's security and privacy policies to maintain entitlements to the service.</span></span>

<span data-ttu-id="228be-112">Автоматические оповещения запускаются при обнаружении подозрительных действий, таких как несколько неудачных входов в систему в течение короткого периода.</span><span class="sxs-lookup"><span data-stu-id="228be-112">Automated alerts trigger when suspicious activity is detected, such as multiple failed logins within a short period.</span></span> <span data-ttu-id="228be-113">Группа реагирования на угрозы безопасности Microsoft 365 использует машинное обучение и анализ больших объемов данных для просмотра и анализа активности, выявления нерегулярных схем доступа и заблаговременного реагирования на аномальные и незаконные действия.</span><span class="sxs-lookup"><span data-stu-id="228be-113">The Microsoft 365 Security Response team uses machine learning and big data analysis to review and analyze activity, look for irregular access patterns, and proactively respond to anomalous and illicit activities.</span></span> <span data-ttu-id="228be-114">Корпорация Майкрософт также использует специальную команду тест-испытателей проникновения и периодически участвует в занятиях "Красная команда" и "Синяя группа" для поиска проблем безопасности и контроля доступа в службе.</span><span class="sxs-lookup"><span data-stu-id="228be-114">Microsoft also employs a dedicated team of penetration testers and engages in periodic Red Team and Blue Team exercises to find security and access control issues in the service.</span></span> <span data-ttu-id="228be-115">Клиенты могут проверить эффективность систем управления доступом с помощью отчетов аудита и API действий управления, предоставляемых Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="228be-115">Customers can verify the effectiveness of access control systems by using audit reports and the management activity API provided by Microsoft 365.</span></span>

<span data-ttu-id="228be-116">Дополнительные сведения см. в справочнике по API действий управления [Office 365,](/office/office-365-management-api/office-365-management-activity-api-reference) аудите и [отчетности в Microsoft 365.](assurance-auditing-and-reporting-overview.md)</span><span class="sxs-lookup"><span data-stu-id="228be-116">For more information, see [Office 365 Management Activity API reference](/office/office-365-management-api/office-365-management-activity-api-reference) and [Auditing and reporting in Microsoft 365](assurance-auditing-and-reporting-overview.md).</span></span>
