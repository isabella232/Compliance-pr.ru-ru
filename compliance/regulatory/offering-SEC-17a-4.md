---
title: Правило 17a-4(f) Комиссии по ценным бумагам и биржам США (США)
description: Независимая компания по оценке проверила, что Azure и Office 365 могут помочь финансовым компаниям соответствовать правилу SEC 17a-4(f) по хранению записей и неуменяемым требованиям к хранилищу.
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
ms.openlocfilehash: f877bbec76cc0d760f2f908975b3818b88551829
ms.sourcegitcommit: 21ed42335efd37774ff5d17d9586d5546147241a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2021
ms.locfileid: "50121208"
---
# <a name="securities-and-exchange-commission-sec-rule-17a-4f-united-states"></a>Правило 17a-4(f) Комиссии по ценным бумагам и биржам США (США)

## <a name="about-sec-rule-17a-4f"></a>О правиле SEC 17a-4(f)

Комиссия по ценным бумагам [и биржам США (SEC)](https://www.sec.gov/) — это независимое агентство федерального правительства США, а также основной контролер и регулятор по рынкам ценных бумаг США. Он контролирует надзор за федеральным законодательством о ценных бумагах, предлагает новые правила ценных бумаг и контролирует регулирование рынка в отрасли ценных бумаг.

SEC определяет строгие и явные требования для регулируемых организаций, которые выбирают хранение книг и записей на электронных носитах. Она установила [17 CFR 240.17a-3](https://www.govinfo.gov/app/details/CFR-2012-title17-vol3/CFR-2012-title17-vol3-sec240-17a-3) и [17 CFR 240.17a-4](https://www.ecfr.gov/cgi-bin/text-idx?mc=true&node=pt17.4.240&rgn=div5#se17.4.240_117a_64) для регулирования регистрации, включая периоды хранения, для брокеров-брокеров ценных бумаг. Позднее SEC [](https://www.sec.gov/rules/interp/34-47806.htm) внес изменения в 17 параграфа CFR 240.17a-4 (f), выпустив два интерпретативных выпуска, чтобы разрешить хранение книг и записей на электронных носитель при условии, что выполнены определенные условия.

Система электронного хранения соответствует этим условиям, если предотвращает изменение или стирание записей в течение требуемого периода хранения. Периоды хранения зависят от трех-шести лет в зависимости от типов записей, при этом в течение первых двух лет должны быть доступны немедленные возможности. Кроме того, один из интерпретативных выпусков требует, чтобы система хранения была способна хранить записи после установленного SEC периода хранения в соответствии с подпунами, юридическим удержанием или другими подобными требованиями.

## <a name="microsoft-and-sec-rule-17a-4f"></a>Правило Майкрософт и SEC 17a-4(f)

Клиенты финансовых услуг, представляющие одну из наиболее жестко регулируемых отраслей в мире, подвержены сложным положениям, таким как хранение финансовых транзакций и связанных коммуникаций в неутираемом и не изумяемом состоянии. Среди наиболее строгих требований является правило 17a-4(f) Комиссии по безопасности и Exchange (SEC) США, которое устанавливает строгие требования для регулируемых организаций, которые выбирают хранение книг и записей на электронном хранилище. Хранимые записи не должны быть изменены или удаляться до окончания указанного периода хранения.

Microsoft Azure Immutable BLOB Storage with Policy Lock and Microsoft Office 365 with Preservation Lock can help financial institutions meet the immutable storage requirements of SEC Rule 17a-4(f).

Чтобы оценить соответствие Azure и Office 365 правилу SEC 17a-4(f), корпорация Майкрософт сохранила независимую компанию по оценке, специализирующуюся на управлении записями и управлении информацией, Cohasset Associates. В итоговом отчете для:

- **Azure**: оценка соответствия требованиям SEC [17a-4(f):](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=19b08fd4-d276-43e8-9461-715981d0ea20&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_GRC_Assessment_Reports)служба хранилища Microsoft Azure ( Cohasset) проверила, что неусвояемое хранилище [BLOB-blob Azure](/azure/storage/blobs/storage-blob-immutable-storage) с параметром блокировки политики, если оно используется для хранения BLOB-данных с учетом времени в неперетираемом и неперезаписаемом формате (WORM), соответствует непеременяемым требованиям правила SEC к хранилищу. Каждый BLOB-проект (запись) защищен от изменения, перезаписи или удаления до истечения требуемого срока хранения и освобождения всех связанных юридических удержаний. Поставщики программного обеспечения и партнеры с конфиденциальными рабочими нагрузками теперь могут использовать неустановимое хранилище BLOB-хранилищ Azure в качестве облачного решения onestop-shop для хранения записей и неуменяемого хранилища. Финансовые учреждения теперь могут создавать собственные приложения, пользуясь преимуществами этих функций, при этом оставаясь совместимыми.
- **Microsoft 365**: для требований [SEC 17a-4(f)](/microsoft-365/compliance/retention-regulatory-requirements#sec-17a-4f-finra-4511c-and-cftc-131c-d) Компания Cohasset проверила, что Microsoft 365 включает функции архивации, которые позволяют регулируемым клиентам, включая брокеров-брокеров, хранить данные таким образом, чтобы они соответствовали требованиям SEC для хранения записей. Функции хранения в Microsoft 365 помогают сохранять широкий спектр данных, включая электронную почту, голосовую почту, общие документы, мгновенные сообщения и сторонние данные. В частности, архивирование в Microsoft 365 позволяет клиентам устанавливать глобальные или детализируемые политики хранения сообщений для хранения данных в течение определенного периода и более длительного периода в неопределяемом и не стираемом формате.

## <a name="microsoft-in-scope-cloud-services"></a>Облачные службы Майкрософт, к которым применима оценка

- [Azure](https://gallery.technet.microsoft.com/Overview-of-Azure-c1be3942)
- [Office 365](https://aka.ms/Office365ComplianceOfferings)

## <a name="audits-reports-and-certificates"></a>Аудит, отчеты и сертификаты

### <a name="azure--sec-rule-17"></a>Azure & SEC Rule 17

[SEC 17a-4(f) & CFTC 1.31 (c-d) Compliance Assessment of Azure Storage](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=19b08fd4-d276-43e8-9461-715981d0ea20&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_GRC_Assessment_Reports)

### <a name="office-365--sec-rule-17"></a>Правило 17 для & SEC в Office 365

[Оценка соответствия требованиям SEC 17a-4(f): Центр безопасности и соответствия требованиям Майкрософт & с SharePoint, OneDrive, Teams, Exchange и Skype для бизнеса](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=9fa8349d-a0c9-47d9-93ad-472aa0fa44ec&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_FAQ_and_White_Papers)

## <a name="how-to-implement"></a>Методика реализации

### <a name="financial-services-regulation"></a>Регулирование финансовых услуг

Карта соответствия основным нормативным принципам США для облачных вычислений и веб-служб Майкрософт. [Подробнее](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides)

### <a name="risk-assessment--compliance-guide"></a>Руководство по оценке & соответствия требованиям

Создайте модель управления для оценки рисков облачных служб Майкрософт и уведомлений регуляторов. [Подробнее](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=edee9b14-3661-4a16-ba83-c35caf672bd7&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_FAQ_and_White_Papers)

### <a name="financial-use-cases"></a>Случаи финансового использования

Используйте обзоры, учебники и другие ресурсы для создания решений Azure для финансовых услуг. [Подробнее](/azure/industry/financial/)

## <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>Оценка риска с помощью диспетчера соответствия требованиям (Майкрософт)

[Диспетчер соответствия требованиям (Майкрософт)](/microsoft-365/compliance/compliance-manager) — это предварительная функция в [Центре соответствия требованиям Microsoft 365](/microsoft-365/compliance/microsoft-365-compliance-center), помогающая понять состояние вашей организации в отношении соответствия требованиям и принять меры по снижению рисков. Диспетчер соответствия требованиям предоставляет премиум-шаблон для оценки этих нормативных требований. Шаблон находится на странице **шаблонов оценки** в диспетчере соответствия требованиям. См. [Создание оценки в диспетчере соответствия требованиям](/microsoft-365/compliance/compliance-manager-assessments).

## <a name="resources"></a>Ресурсы

- [Архив в Microsoft Office 365, хранение данных и правило 17a-4](https://www.microsoft.com/microsoft-365/blog/2015/11/10/office-365-exchange-online-archiving-now-meets-sec-rule-17a-4-requirements/)
- [Соответствие требованиям финансовых служб Майкрософт](https://download.microsoft.com/download/6/4/7/64707E3E-6D3E-45D0-8207-A0EA3201B4A6/Microsoft%20Cloud%20-%20Financial%20Services%20Compliance%20Program%20\(Print\).pdf)
- [Программа соответствия требованиям: облачные и финансовые службы Майкрософт для бизнеса](https://servicetrust.microsoft.com/viewpage/financialservicesoverview)
- [Соответствие финансовых услуг требованиям в Azure](https://azure.microsoft.com/resources/videos/azurecon-2015-financial-services-compliance-in-azure/)
- [Средство оценки облачных рисков для финансовых услуг в Azure](https://servicetrust.microsoft.com/ViewPage/FFIECBlueprint?command=Download&downloadType=Document&downloadId=079a1973-711a-428f-9312-9ddd290cff7b&docTab=c726d5c0-2d1e-11e8-a485-57140ec19669_PaaS)
- [Microsoft Office 365 Retention Policies](/office365/securitycompliance/retention-policies)
- [Сообщество финансовых услуг Майкрософт](https://techcommunity.microsoft.com/t5/financial-services/ct-p/FinancialServices)
- [Соответствие требованиям в центре управления безопасностью Майкрософт](https://www.microsoft.com/trust-center/compliance/compliance-overview)
