---
title: Правило 17a-4(f) Комиссии по ценным бумагам и Exchange (SEC) США
description: Независимая фирма по оценке подтвердила, что Azure и Office 365 могут помочь финансовым фирмам выполнить правила SEC 17a-4(f) хранения записей и неоменяемых требований к хранению.
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
ms.openlocfilehash: d92fc7b56d2c240588b90afad6a82264fde911c5
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2021
ms.locfileid: "53384329"
---
# <a name="securities-and-exchange-commission-sec-rule-17a-4f-united-states"></a>Правило 17a-4(f) Комиссии по ценным бумагам и Exchange (SEC) США

## <a name="about-sec-rule-17a-4f"></a>О правиле SEC 17a-4(f)

Комиссия по ценным бумагам и Exchange США [(SEC)](https://www.sec.gov/) является независимым агентством федерального правительства США и главным контролером и регулятором рынков ценных бумаг США. Он обладает правоприменительных полномочий над федеральными законами о ценных бумагах, предлагает новые правила ценных бумаг и контролирует регулирование рынка в отрасли ценных бумаг.

SEC определяет строгие и четкие требования к регулируемым субъектам, которые выбирают для хранения книг и записей на электронных носитах хранения. Она установила [17 CFR 240.17a-3](https://www.govinfo.gov/app/details/CFR-2012-title17-vol3/CFR-2012-title17-vol3-sec240-17a-3) и [17 CFR 240.17a-4](https://www.ecfr.gov/cgi-bin/text-idx?mc=true&node=pt17.4.240&rgn=div5#se17.4.240_117a_64) для регулирования ведения записей, включая периоды хранения, для брокеров-дилеров ценных бумаг. Позднее SEC внесла изменения в [пункт](https://www.sec.gov/rules/interp/34-47806.htm) 17 CFR 240.17a-4 (f), издав два выпуска интерпретации, чтобы разрешить хранить книги и записи в средствах электронного хранения до тех пор, пока будут выполнены определенные условия.

Электронная система хранения отвечает этим условиям, если она предотвращает изменение или стирание записей в течение необходимого периода хранения. Срок хранения варьируется от трех до шести лет в зависимости от типов записей, при этом для первых двух лет требуется немедленная доступность. Кроме того, для одного из выпусков интерпретации необходимо, чтобы система хранения была способна хранить записи за пределами установленного SEC периода хранения, чтобы соответствовать требованиям по повесткам, юридическому удержанию или другим подобным требованиям.

## <a name="microsoft-and-sec-rule-17a-4f"></a>Правило Microsoft и SEC 17a-4(f)

Клиенты финансовых служб, представляющие одну из наиболее строго регулируемых отраслей в мире, подвержены сложным положениям, таким как хранение финансовых транзакций и связанных с ними сообщений в неустанных и неустанных состояниях. Среди наиболее предписывающих является правило 17a-4(f) Комиссии по безопасности и безопасности США Exchange (SEC), которое предусматривает строгие требования к регулируемым организациям, которые выбирают для хранения книг и записей на электронных носитлях хранения. Записи, хранимые, должны быть ненадеженными без возможности изменять или удалять их до окончания назначенного периода хранения.

Microsoft Azure Непередаваемые Blob служба хранилища с блокировкой политики и Microsoft Office 365 с блокировкой сохранения могут помочь финансовым учреждениям соответствовать непеременяемым требованиям хранения правила SEC 17a-4(f).

Чтобы оценить соответствие Azure и Office 365 правилу SEC 17a-4(f), Корпорация Майкрософт сохранила независимую фирму по оценке, которая специализируется на управлении записями и управлении информацией, Cohasset Associates. В итоговом отчете для:

- **Azure**: [SEC 17a-4(f)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=19b08fd4-d276-43e8-9461-715981d0ea20&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_GRC_Assessment_Reports)Оценка соответствия требованиям: служба хранилища Microsoft Azure , Cohasset подтвердила, что [Azure Immutable Blob служба хранилища](/azure/storage/blobs/storage-blob-immutable-storage) с параметром Блокировка политики, когда используется для сохранения временного Blobs в неустанном и неописуемом формате (WORM), отвечает непеременяемым требованиям к хранению правила SEC. Каждый Blob (запись) защищен от изменения, перезаписи или удаления, пока не истечет необходимый период хранения и не будут выпущены все связанные юридические удержания. Поставщики программного обеспечения и партнеры с конфиденциальными рабочими нагрузками теперь могут использовать Azure Immutable Blob служба хранилища как облачное решение onestop-shop для хранения записей и неостановимого хранения. Финансовые учреждения теперь могут создавать собственные приложения, пользуясь этими функциями, оставаясь совместимыми.
- **Microsoft 365.** Для требований [SEC 17a-4(f)](/microsoft-365/compliance/retention-regulatory-requirements#sec-17a-4f-finra-4511c-and-cftc-131c-d) Cohasset подтвердил, что Microsoft 365 включает функции архивации, которые позволяют регулируемым клиентам, включая брокеров-дилеров, хранить данные таким образом, чтобы они соответствовали требованиям SEC для хранения записей. Функции хранения Microsoft 365 сохраняют широкий спектр данных, включая электронную почту, голосовую почту, общие документы, мгновенные сообщения и сторонние данные. В частности, архивирование в Microsoft 365 позволяет клиентам устанавливать глобальные или гранулярные политики хранения сообщений для хранения данных за определенный период и за его пределами в неописуемом, не стираемом формате.

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Облачные платформы Microsoft в области & служб

- [Azure](https://gallery.technet.microsoft.com/Overview-of-Azure-c1be3942)
- [Office 365](https://aka.ms/Office365ComplianceOfferings)

## <a name="audits-reports-and-certificates"></a>Аудит, отчеты и сертификаты

### <a name="azure--sec-rule-17"></a>Azure & SEC Rule 17

[Sec 17a-4(f) & CFTC 1.31 (c-d) Оценка соответствия требованиям служба хранилища Azure](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=19b08fd4-d276-43e8-9461-715981d0ea20&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_GRC_Assessment_Reports)

### <a name="office-365--sec-rule-17"></a>Office 365 & SEC Rule 17

[Оценка соответствия требованиям SEC 17a-4(f): Центр соответствия требованиям & microsoft Security SharePoint, OneDrive, Teams, Exchange и Skype для бизнеса](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=2dc92867-5f83-49d8-ad04-9e7295c9e40e&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_FAQ_and_White_Papers)

## <a name="how-to-implement"></a>Методика реализации

### <a name="financial-services-regulation"></a>Регулирование финансовых служб

Карта соответствия ключевым принципам регулирования США для облачных вычислений и онлайн-служб Microsoft. [Подробнее](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides)

### <a name="risk-assessment--compliance-guide"></a>Руководство по оценке & соответствия требованиям

Создание модели управления для оценки рисков облачных служб Майкрософт и уведомления регулятора. [Подробнее](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=edee9b14-3661-4a16-ba83-c35caf672bd7&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_FAQ_and_White_Papers)

### <a name="financial-use-cases"></a>Случаи финансового использования

Используйте обзоры кейсов, учебники и другие ресурсы для создания решений Azure для финансовых служб. [Подробнее](/azure/industry/financial/)

## <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>Оценка риска с помощью диспетчера соответствия требованиям (Майкрософт)

[Диспетчер соответствия требованиям (Майкрософт)](/microsoft-365/compliance/compliance-manager) — это предварительная функция в [Центре соответствия требованиям Microsoft 365](/microsoft-365/compliance/microsoft-365-compliance-center), помогающая понять состояние вашей организации в отношении соответствия требованиям и принять меры по снижению рисков. Диспетчер соответствия требованиям предоставляет премиум-шаблон для оценки этих нормативных требований. Шаблон находится на странице **шаблонов оценки** в диспетчере соответствия требованиям. См. [Создание оценки в диспетчере соответствия требованиям](/microsoft-365/compliance/compliance-manager-assessments).

## <a name="resources"></a>Ресурсы

- [Архивативная Microsoft Office 365, хранение данных и правило 17a-4](https://www.microsoft.com/microsoft-365/blog/2015/11/10/office-365-exchange-online-archiving-now-meets-sec-rule-17a-4-requirements/)
- [Соответствие требованиям Microsoft Financial Services](https://download.microsoft.com/download/6/4/7/64707E3E-6D3E-45D0-8207-A0EA3201B4A6/Microsoft%20Cloud%20-%20Financial%20Services%20Compliance%20Program%20\(Print\).pdf)
- [Программа соответствия требованиям облачные службы и финансовые службы Майкрософт для бизнеса](https://servicetrust.microsoft.com/viewpage/financialservicesoverview)
- [Соответствие финансовых услуг требованиям в Azure](https://azure.microsoft.com/resources/videos/azurecon-2015-financial-services-compliance-in-azure/)
- [Средство оценки облачных рисков для финансовых услуг в Azure](https://servicetrust.microsoft.com/ViewPage/FFIECBlueprint?command=Download&downloadType=Document&downloadId=079a1973-711a-428f-9312-9ddd290cff7b&docTab=c726d5c0-2d1e-11e8-a485-57140ec19669_PaaS)
- [Microsoft Office 365 Политики хранения](/office365/securitycompliance/retention-policies)
- [Microsoft Financial Services Community](https://techcommunity.microsoft.com/t5/financial-services/ct-p/FinancialServices)
- [Соответствие требованиям в центре управления безопасностью Майкрософт](https://www.microsoft.com/trust-center/compliance/compliance-overview)
