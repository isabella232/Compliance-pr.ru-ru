---
title: Системный и организационный контроль (SOC) 3
description: Узнайте как облачные службы (Майкрософт) соответствуют стандартам системного и организационного контроля (SOC) 3 для операционной безопасности.
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
ms.openlocfilehash: b3690ba79ba8adca1d01e4eda03831c431747d01
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/23/2021
ms.locfileid: "58481081"
---
# <a name="system-and-organization-controls-soc-3"></a>Системный и организационный контроль (SOC) 3

## <a name="soc-3-overview"></a>Обзор SOC 3

Системный и организационный контроль (SOC) для обслуживающих организаций — это отчеты о внутреннем контроле, созданные Американским институтом дипломированных общественных бухгалтеров (AICPA). Они предназначены для проверки служб, предоставляемых обслуживающей организацией, чтобы конечные пользователи могли оценить и устранить риски, связанные с внешней службой.

*SOC 3 SOC для обслуживающих организаций: Критерии доверительных служб для отчетов общего пользования* — это краткая общедоступная версия отчета об аттестации SOC 2 типа 2 для пользователей, которым требуются гарантии в отношении средств управления обслуживающей организацией, относящиеся к безопасности, доступности, целостности обработки и конфиденциальности, но не требуется полный отчет SOC 2. Так как отчеты SOC 3 являются отчетами общего пользования, их можно свободно распространять.

Отчет SOC 3 содержит письменное утверждение руководства обслуживающей организации относительно эффективности контроля для достижения обязательств на основе применимых критериев доверительных служб а также мнение аудитора обслуживания о том, справедливо ли заявление руководства.

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Затрагиваемые облачные платформы и службы Майкрософт

Затрагиваемые службы Майкрософт показаны в отчете об [аттестации SOC 2 типа 2](offering-soc-2.md) Azure.

- Azure (подробные сведения см. в разделе [Предложения по обеспечению соответствия требованиям Microsoft Azure](https://azure.microsoft.com/resources/microsoft-azure-compliance-offerings/) или отчете об оценке Azure SOC 2 (тип 2))
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

## <a name="azure-dynamics-365-and-soc-3"></a>Azure, Dynamics 365 и SOC 3

Дополнительные сведения о соответствии требованиям Azure, Dynamics 365 и другим веб-службам см. в разделе [Предложение Azure SOC 3](/azure/compliance/offerings/offering-soc-3).

## <a name="office-365-and-soc-3"></a>Office 365 и SOC 3

### <a name="office-365-cloud-environments"></a>Облачные среды Office 365

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Применимость Office 365 и затрагиваемые службы

Чтобы определить применимость служб и подписки Office 365, используйте следующую таблицу.

| **Применимость** | **Затрагиваемые службы** |
|:------------------|:----------------------|
| **Коммерческий сектор** | Диспетчер соответствия требованиям, защищенное хранилище, Delve, Exchange Online Protection, Exchange Online, Forms, Griffin, Identity Manager, Lockbox (Torus), Microsoft Teams, MyAnalytics, клиентский портал Office 365, микрослужбы Office 365, в том числе Kaizala, ObjectStore, Sway, служба документов PowerPoint Online, служба аннотации запросов, Синхронизация сведений о школе, Siphon, Speech, StaffHub, программа приложений eXtensible, Office Online, инфраструктура служб Office, OneDrive для бизнеса, Планировщик, PowerApps, Power Automate, Power BI, Project Online, шифрование службы с помощью ключа клиента, SharePoint Online, Skype для бизнеса |
| **GCC** | Azure Active Directory, диспетчер соответствия требованиям, Delve, Exchange Online, 
, Microsoft Defender для Office 365, Microsoft Teams, MyAnalytics, надстройка Office 365 Advanced Compliance, Центр безопасности и соответствия требованиям Office 365, Office Online, Office Pro Plus, OneDrive для бизнеса, Планировщик, PowerApps, Power Automate, Power BI, SharePoint Online, Skype для бизнеса, Stream |
| **GCC High** | Azure Active Directory, Exchange Online, Flow, Microsoft Defender для Office 365, Microsoft Teams, надстройка Office 365 Advanced Compliance, Центр безопасности и соответствия требованиям Office 365, Office Online, Office Pro Plus, OneDrive для бизнеса, Планировщик, PowerApps, Power Automate, Power BI, SharePoint Online, Skype для бизнеса |
| **DoD** | Azure Active Directory, Exchange Online, Microsoft Defender для Office 365, Microsoft Teams, надстройка Office 365 Advanced Compliance, Центр безопасности и соответствия требованиям Office 365, Office Online, Office Pro Plus, OneDrive для бизнеса, Планировщик, Power Automate, Power BI, SharePoint Online, Skype для бизнеса |

### <a name="office-365-audit-reports"></a>Отчеты аудита Office 365

- [Отчет SOC 3 (SSAE 18) для Office 365 Core](https://aka.ms/o365SOC-3)
- [См. связывающие письма и дополнительные отчеты аудита](https://aka.ms/auditreports)

У вас должна быть существующая подписка или бесплатная пробная учетная запись в Office 365 или Office 365 для государственных организаций США, чтобы скачивать отчеты об аттестации SOC 1 и SOC 2 и любые промежуточные письменные заверения по мере необходимости.

### <a name="frequently-asked-questions"></a>Вопросы и ответы

**Как часто выпускаются отчеты SOC для Office 365?**

Отчеты SOC для Office 365 и других сетевых служб основаны на скользящем 12-месячном периоде выполнения (период аудита) с выпуском новых отчетов раз в полгода (конец периода — 31 марта и 30 сентября). *Письма об увязке условий* выпускаются каждый квартал и охватывают предыдущий трехмесячный период. Например, январское письменное заверение охватывает период с 1 октября по 31 декабря, апрельское письменное заверение охватывает период с 1 января по 31 марта, июльское письменное заверение охватывает период с 1 апреля по 30 июня, а октябрьское письменное заверение охватывает период с 1 июля по 30 сентября.

**Где можно получить документацию по аудиту SOC для Office 365, включая промежуточное письменное заверение?** Ссылки на документацию по аудиту см. в разделе отчета об аудите. Для входа у вас должна быть существующая подписка или бесплатная пробная учетная запись в Office 365 или [Office](https://azure.microsoft.com/global-infrastructure/government/request/)365 для государственных организаций США. Затем вы можете скачать сертификаты аудита, отчеты об оценке и другие соответствующие документы, которые помогут вам с собственными нормативными требованиями.

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>Оценка риска с помощью диспетчера соответствия требованиям (Майкрософт)

[Диспетчер соответствия требованиям (Майкрософт)](/microsoft-365/compliance/compliance-manager) — это предварительная функция в [Центре соответствия требованиям Microsoft 365](/microsoft-365/compliance/microsoft-365-compliance-center), помогающая понять состояние вашей организации в отношении соответствия требованиям и принять меры по снижению рисков. Диспетчер соответствия требованиям предоставляет премиум-шаблон для оценки этих нормативных требований. Шаблон находится на странице **шаблонов оценки** в диспетчере соответствия требованиям. См. [Создание оценки в диспетчере соответствия требованиям](/microsoft-365/compliance/compliance-manager-assessments).

### <a name="resources"></a>Ресурсы

- [Отчеты об аудите Service Trust Portal](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3)
- [AICPA SOC для обслуживающих организаций](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/socforserviceorganizations.html)
- [SSAE № 18 — "Стандарты аттестации: уточнение и повторная кодификация (профессиональные стандарты AICPA)"](https://www.aicpa.org/Research/Standards/AuditAttest/DownloadableDocuments/SSAE_No_18.pdf)
- [Отчет SOC 2 по проверке элементов управления в обслуживающей организации, относящихся к безопасности, доступности, целостности обработки или конфиденциальности (Руководство AICPA)](https://future.aicpa.org/cpe-learning/publication/soc-2-reporting-on-an-examination-of-controls-at-a-service-organization-relevant-to-security-availability-processing-integrity-confidentiality-or-privacy-OPL) (можно приобрести)
- [Раздел 100 TSP (AICPA, 2017: критерии доверительных служб)](https://www.aicpa.org/content/dam/aicpa/interestareas/frc/assuranceadvisoryservices/downloadabledocuments/trust-services-criteria.pdf)
