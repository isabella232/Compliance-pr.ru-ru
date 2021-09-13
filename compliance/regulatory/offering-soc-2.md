---
title: Системный и организационный контроль 2, тип 2
description: Узнайте как облачные службы (Майкрософт) соответствуют стандартам системного и организационного контроля (SOC) 2, типа 2 для операционной безопасности.
keywords: Microsoft 365, соответствие требованиям, предложения
ms.localizationpriority: high
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
ms.openlocfilehash: 92fb47f98e60eb655ee68b38cb747a7d2eb9d2ff
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59161243"
---
# <a name="system-and-organization-controls-soc-2-type-2"></a>Системный и организационный контроль 2, тип 2

## <a name="soc-2-type-2-overview"></a>Обзор SOC 2, тип 2

Системный и организационный контроль (SOC) для обслуживающих организаций— это отчеты о внутреннем контроле, созданные Американским институтом дипломированных общественных бухгалтеров (AICPA). Они предназначены для проверки служб, предоставляемых обслуживающейся организацией, чтобы конечные пользователи могли оценить и устранить риски, связанные с внешней службой.

Аттестация SOC 2, тип 2 выполняется при следующих условиях:

- SSAE № 18 "Стандарты аттестации: уточнение и повторная кодификация", включающий раздел 105 AT-C — *Основные понятия, общие для всех обязательств по аттестации* и раздел 205 AT-C — *Обязательства по аттестации* (AICPA, профессиональные стандарты).
- Отчет SOC 2 по проверке элементов управления в обслуживающей организации, относящихся к безопасности, доступности, целостности обработки или конфиденциальности (Руководство AICPA).
- Раздел TSP 100, 2017 Критерии служб доверия для безопасности, доступности, целостности обработки и конфиденциальности (AICPA, критерии служб доверия 2017).

Кроме того, отчет об аттестации Office 365 SOC 2, тип 2 соответствует требованиям, изложенным в Матрице управления облачными средствами управления (CCM) Cloud Security Alliance (CSA) и Каталоге критериев соответствия облачных вычислений (C5: 2020), созданном Федеральным ведомством Германии по информационной безопасности (BSI).

Аттестации SOC 2 Office 365 основаны на строгих независимых сторонних аудитах, проводимых авторитетной фирмой CPA. В завершении аудита SOC 2 аудитор формирует заключение в отчете SOC 2 (тип 2), в котором описывается система CSP и оценивается объективность облачного поставщика службы CSP в описании своих средств контроля. В нем также оценивается соответствие назначения средств контроля CSP; работали ли они в указанную дату и были ли эффективны в определенный период времени. Отчеты SOC 2 (тип 2) в Office 365 имеют отношение к безопасности, доступности, целостности обработки и конфиденциальности системы.

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Затрагиваемые облачные платформы и службы Майкрософт

Веб-службы Майкрософт в области показаны в отчете об аттестации Azure SOC 2 (тип 2):

- Azure (подробные сведения см. в разделе [Предложения по обеспечению соответствия требованиям Microsoft Azure](https://azure.microsoft.com/resources/microsoft-azure-compliance-offerings/) или отчете об оценке Azure SOC 2 (тип 2))
- Azure DevOps (см. отдельный отчет по проверке Azure DevOps SOC 2 (тип 2))
- Dynamics 365 (подробные сведения см. в отчете об аттестации Azure SOC 2 (тип 2))
- Microsoft 365 Defender
- Microsoft Cloud App Security (MCAS)
- Microsoft Defender для конечной точки
- Microsoft Defender для удостоверений
- Microsoft Forms Pro (не входит в область Azure для государственных организаций)
- Microsoft Graph
- Microsoft Intune
- Компьютеры, управляемые Майкрософт (не входит в область Azure для государственных организаций)
- Microsoft Stream
- Эксперты Майкрософт по угрозам (не входит в область Azure для государственных организаций)
- Портал назначения
- Office 365, Office 365 для государственных организаций США, Office 365 для государственных организаций США — высокий уровень, Office 365 для министерства обороны США
- Power Apps
- Power Automate
- Power BI
- Power Virtual Agents (не входит в область Azure для государственных организаций)
- Соответствие обновлений требованиям (не входит в область Azure для государственных организаций)

## <a name="azure-dynamics-365-and-soc-2"></a>Azure, Dynamics 365 и SOC 2

Дополнительные сведения о соответствии требованиям Azure, Dynamics 365 и другим веб-службам см. в разделе [Предложение Azure SOC 2](/azure/compliance/offerings/offering-soc-2).

## <a name="office-365-and-soc-2"></a>Office 365 и SOC 2

### <a name="office-365-cloud-environments"></a>Облачные среды Office 365

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Применимость Office 365 и затрагиваемые службы

Чтобы определить применимость изменений к вашим службам и подписке Office 365, воспользуйтесь следующей таблицей.

| **Применимость** | **Затрагиваемые службы** |
|:------------------|:----------------------|
| **Коммерческий сектор** | Диспетчер соответствия требованиям, защищенное хранилище, Delve, Exchange Online Protection, Exchange Online, Forms, Griffin, Identity Manager, Lockbox (Torus), Microsoft Teams, MyAnalytics, клиентский портал Office 365, микрослужбы Office 365, в том числе Kaizala, ObjectStore, Sway, служба документов PowerPoint Online, служба аннотации запросов, Синхронизация сведений о школе, Siphon, Speech, StaffHub, программа приложений eXtensible, Office Online, инфраструктура служб Office, OneDrive для бизнеса, Планировщик, PowerApps, Power Automate, Power BI, Project Online, шифрование службы с помощью ключа клиента, SharePoint Online, Skype для бизнеса |
| **GCC** | Azure Active Directory, диспетчер соответствия требованиям, Delve, Exchange Online, Forms, Microsoft Defender для Office 365, Microsoft Teams, MyAnalytics, надстройка Office 365 Advanced Compliance, Центр безопасности и соответствия требованиям Office 365, Office Online, Office Pro Plus, OneDrive для бизнеса, Планировщик, PowerApps, Power Automate, Power BI, SharePoint Online, Skype для бизнеса, Stream |
| **GCC High** | Azure Active Directory, Exchange Online, Forms, Microsoft Defender для Office 365, Microsoft Teams, надстройка Office 365 Advanced Compliance, Центр безопасности и соответствия требованиям Office 365, Office Online, Office Pro Plus, OneDrive для бизнеса, Планировщик, PowerApps, Power Automate, Power BI, SharePoint Online, Skype для бизнеса |
| **DoD** | Azure Active Directory, Exchange Online, Forms, Microsoft Defender для Office 365, Microsoft Teams, надстройка Office 365 Advanced Compliance, Центр безопасности и соответствия требованиям Office 365, Office Online, Office Pro Plus, OneDrive для бизнеса, Планировщик, Power BI, SharePoint Online, Skype для бизнеса |

### <a name="office-365-audit-reports"></a>Отчеты аудита Office 365

- [Отчет SOC 2 (SSAE 18) для Office 365 Core](https://aka.ms/o365SOC-2)
- [Отчет SOC 2 (T1-SSAE 18, тип I) для микрослужб Office 365](https://aka.ms/o365-MS-SOC-2-type1)
- [См. связывающие письма и дополнительные отчеты аудита](https://aka.ms/auditreports)

У вас должна быть существующая подписка или бесплатная пробная учетная запись в Office 365 или [Office](https://azure.microsoft.com/global-infrastructure/government/request/) 365 для государственных организаций США, чтобы скачивать отчеты об аттестации SOC 1 и SOC 2 и любые промежуточные письменные заверения по мере необходимости.

### <a name="frequently-asked-questions"></a>Вопросы и ответы

**Как часто выпускаются отчеты SOC для Office 365?**

Отчеты SOC для Office 365 и других сетевых служб основаны на скользящем 12-месячном периоде выполнения (период аудита) с выпуском новых отчетов раз в полгода (конец периода — 31 марта и 30 сентября). *Письма об увязке условий* выпускаются каждый квартал и охватывают предыдущий трехмесячный период. Например, январское письменное заверение охватывает период с 1 октября по 31 декабря, апрельское письменное заверение охватывает период с 1 января по 31 марта, июльское письменное заверение охватывает период с 1 апреля по 30 июня, а октябрьское письменное заверение охватывает период с 1 июля по 30 сентября.

**Где можно получить документацию по аудиту SOC для Office 365, включая промежуточное письменное заверение?**

Ссылки на документацию по аудиту см. в разделе отчета об аудите. Для входа у вас должна быть существующая подписка или бесплатная пробная учетная запись в Office 365 или [Office](https://azure.microsoft.com/global-infrastructure/government/request/)365 для государственных организаций США. Затем вы можете скачать сертификаты аудита, отчеты об оценке и другие соответствующие документы, которые помогут вам с собственными нормативными требованиями.

**Где можно найти оценку реализации элементов управления CCM Cloud Security Alliance?**

Аудит SOC 2 типа 2 для Office 365 основан на принципах и критериях служб доверия Американского института дипломированных присяжных бухгалтеров (AICPA), включая безопасность, доступность, конфиденциальность, целостность обработки и условия в матрице управления облачными элементами управления (CCM) Cloud Security Alliance (CSA). Цель состоит в соблюдении условий AICPA и требований, указанных в CCM. Аудит SOC 2 типа 2 для Office 365 включает оценку элементов управления CCM, требуемую аттестацией CSA STAR. Дополнительные сведения см. в отчете об аттестации SOC 2 типа 2 для Office 365.

**Где можно увидеть ответы руководства на отмеченные исключения?**

Ответы руководства находятся ближе к концу отчета о результатах аудита SOC. Выполните поиск в документе по запросу "Ответ руководства".

**Где можно ознакомиться с обязанностями организации-пользователя?**

Обязанности субъектов-пользователей указаны в самом конце отчета о результатах аудита SOC. Выполните поиск в документе по запросу "Обязанности организаций-пользователей".

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>Оценка риска с помощью диспетчера соответствия требованиям (Майкрософт)

[Диспетчер соответствия требованиям (Майкрософт)](/microsoft-365/compliance/compliance-manager) — это предварительная функция в [Центре соответствия требованиям Microsoft 365](/microsoft-365/compliance/microsoft-365-compliance-center), помогающая понять состояние вашей организации в отношении соответствия требованиям и принять меры по снижению рисков. Диспетчер соответствия требованиям предоставляет премиум-шаблон для оценки этих нормативных требований. Шаблон находится на странице **шаблонов оценки** в диспетчере соответствия требованиям. См. [Создание оценки в диспетчере соответствия требованиям](/microsoft-365/compliance/compliance-manager-assessments).

### <a name="resources"></a>Ресурсы

- [Отчеты об аудите Service Trust Portal](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3)
- [AICPA SOC для обслуживающих организаций](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/socforserviceorganizations.html)
- [SSAE № 18 — "Стандарты аттестации: уточнение и повторная кодификация (профессиональные стандарты AICPA)"](https://www.aicpa.org/Research/Standards/AuditAttest/DownloadableDocuments/SSAE_No_18.pdf)
- [Отчет SOC 2 по проверке элементов управления в обслуживающей организации, относящихся к безопасности, доступности, целостности обработки или конфиденциальности (Руководство AICPA)](https://future.aicpa.org/cpe-learning/publication/soc-2-reporting-on-an-examination-of-controls-at-a-service-organization-relevant-to-security-availability-processing-integrity-confidentiality-or-privacy-OPL) (можно приобрести)
- [Раздел 100 TSP (AICPA, 2017: критерии доверительных служб)](https://www.aicpa.org/content/dam/aicpa/interestareas/frc/assuranceadvisoryservices/downloadabledocuments/trust-services-criteria.pdf)
