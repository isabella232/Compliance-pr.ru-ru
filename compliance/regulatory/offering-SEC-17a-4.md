---
title: Правило 17a-4(f) Комиссии по ценным бумагам и Exchange (SEC) США
description: Независимая фирма по оценке подтвердила, что Azure и Office 365 могут помочь финансовым фирмам выполнить правила SEC 17a-4(f) хранения записей и неоменяемых требований к хранению.
keywords: Microsoft 365, соответствие требованиям, предложения
ms.localizationpriority: medium
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
ms.openlocfilehash: 50c44b6801e15af02bf4bfa4f4d46758b7a6c7a8
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59161179"
---
# <a name="securities-and-exchange-commission-sec-rule-17a-4f-united-states"></a>Правило 17a-4(f) Комиссии по ценным бумагам и Exchange (SEC) США

## <a name="about-sec-rule-17a-4f"></a>О правиле SEC 17a-4(f)

Комиссия по ценным бумагам и Exchange США [(SEC)](https://www.sec.gov/) является независимым агентством федерального правительства США и главным контролером и регулятором рынков ценных бумаг США. Он обладает правоприменительных полномочий над федеральными законами о ценных бумагах, предлагает новые правила ценных бумаг и контролирует регулирование рынка в отрасли ценных бумаг.

SEC определяет строгие и четкие требования к регулируемым субъектам, которые выбирают для хранения книг и записей на электронных носитах хранения. Она установила [17 CFR 240.17a-3](https://www.govinfo.gov/app/details/CFR-2012-title17-vol3/CFR-2012-title17-vol3-sec240-17a-3) и [17 CFR 240.17a-4](https://www.ecfr.gov/cgi-bin/text-idx?mc=true&node=pt17.4.240&rgn=div5#se17.4.240_117a_64) для регулирования ведения записей, включая периоды хранения, для брокеров-дилеров ценных бумаг. Позднее SEC внесла изменения в [пункт](https://www.sec.gov/rules/interp/34-47806.htm) 17 CFR 240.17a-4 (f), издав два выпуска интерпретации, чтобы разрешить хранить книги и записи в средствах электронного хранения до тех пор, пока будут выполнены определенные условия.

Электронная система хранения отвечает этим условиям, если она предотвращает изменение или стирание записей в течение необходимого периода хранения. Срок хранения варьируется от трех до шести лет в зависимости от типов записей, при этом для первых двух лет требуется немедленная доступность. Кроме того, для одного из выпусков интерпретации необходимо, чтобы система хранения была способна хранить записи за пределами установленного SEC периода хранения, чтобы соответствовать требованиям по повесткам, юридическому удержанию или другим подобным требованиям.

## <a name="microsoft-and-sec-rule-17a-4f"></a>Правило Microsoft и SEC 17a-4(f)

Клиенты финансовых служб, представляющие одну из наиболее строго регулируемых отраслей в мире, подвержены сложным положениям, таким как хранение финансовых транзакций и связанных с ними сообщений в неустанных и неустанных состояниях. Среди наиболее предписывающих является правило 17a-4(f) Комиссии по безопасности и безопасности США Exchange (SEC), которое предусматривает строгие требования к регулируемым организациям, которые выбирают для хранения книг и записей на электронных носитлях хранения. Записи, хранимые, должны быть ненадеженными без возможности изменять или удалять их до окончания назначенного периода хранения.

Microsoft Azure Непередаваемые Blob служба хранилища с блокировкой политики и Microsoft Office 365 с блокировкой сохранения могут помочь финансовым учреждениям соответствовать непеременяемым требованиям хранения правила SEC 17a-4(f).

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Затрагиваемые облачные платформы и службы Майкрософт

- [Azure](https://gallery.technet.microsoft.com/Overview-of-Azure-c1be3942)
- [Office 365](https://aka.ms/Office365ComplianceOfferings)

## <a name="independent-assessments"></a>Независимые оценки

Чтобы оценить соответствие Azure и Office 365 правилу SEC 17a-4(f), Корпорация Майкрософт сохранила независимую фирму по оценке, которая специализируется на управлении записями и управлении информацией, Cohasset Associates.

### <a name="azure"></a>Azure

[Неоменяемое](/azure/storage/blobs/storage-blob-immutable-storage) хранилище для хранилища Azure Blob позволяет пользователям хранить критически важные для бизнеса записи в состоянии записи после чтения многих (WORM). Это состояние делает данные неустанными и не модификабельными для указанного пользователем интервала. На протяжении интервала хранения blob можно создавать и читать, но нельзя изменять или удалять. Эти функции неоменяемого хранилища Azure могут помочь клиентам в решении их требований к хранению записей.

Корпорация Майкрософт сохранила независимую сторонную фирму по оценке, которая специализируется на управлении записями и управлении информацией для оценки неоменяемого хранения для хранения хранилищ Azure Blob с требованиями правила SEC 17a-4(f). В результате отчет *[Cohasset Assessment: Microsoft Azure WORM служба хранилища](https://azure.microsoft.com/resources/azure-immutable-storage-assessment-for-sec-17a-4f-by-cohasset/)* доступен для клиентов.

По мнению оценителя, служба хранилища Azure с непеременяемым хранилищем для функции  *Blobs Azure* и заблокированным вариантом политики на основе времени сохраняет Blobs (записи) на основе времени в неперетираемом и неперезаписываемом. формат и соответствующие требованиям к хранению правила SEC 17a-4(f), [правила FINRA 4511(c)](offering-FINRA-4511.md)и требований правила [CFTC 1.31 (c)-d)](offering-cftc-1-31-us.md).

По запросу корпорация Майкрософт также предоставит *90-дневное* письмо, необходимое для удовлетворения требований SEC 17a-4(f)(2) для клиентов, чтобы уведомить об этом назначенный орган проверки не менее чем за 90 дней до использования средств хранения электронных данных. Как указано в правилах, "член, брокер или дилер должен предоставить свое собственное представление или одно от поставщика среды хранения или другого третьего участника с соответствующими знаниями о том, что выбранные носителя хранения соответствуют условиям, установленным в этом абзаце (f)(2)." Чтобы получить microsoft *Attestation of Electronic служба хранилища Cлужбы мультимедиа* для sec Rule 17a-4, [](https://azure.microsoft.com/support/create-ticket/) клиенты с планом поддержки [Azure](https://azure.microsoft.com/support/plans/) могут создать билет поддержки на портале Azure и запросить письмо для проверки для правила SEC 17a-4. В этом документе Корпорация Майкрософт предоставляет гарантии, соответствующие требованиям SEC 17a-4(f)(2).

### <a name="office-365"></a>Office 365

Для требований [SEC 17a-4(f)](/microsoft-365/compliance/retention-regulatory-requirements#sec-17a-4f-finra-4511c-and-cftc-131c-d) Cohasset подтвердил, что Microsoft 365 включает функции архивации, которые позволяют регулируемым клиентам, в том числе брокерам-дилерам, хранить данные таким образом, чтобы они соответствовали требованиям SEC для хранения записей. Функции хранения Microsoft 365 сохраняют широкий спектр данных, включая электронную почту, голосовую почту, общие документы, мгновенные сообщения и сторонние данные. В частности, архивирование в Microsoft 365 позволяет клиентам устанавливать глобальные или гранулярные политики хранения сообщений для хранения данных за определенный период и за его пределами в неописуемом, не стираемом формате.

## <a name="audits-reports-and-certificates"></a>Аудит, отчеты и сертификаты

### <a name="azure--sec-rule-17"></a>Azure & SEC Rule 17

- [Sec 17a-4(f) & CFTC 1.31 (c-d) Оценка соответствия требованиям служба хранилища Azure](https://azure.microsoft.com/resources/azure-immutable-storage-assessment-for-sec-17a-4f-by-cohasset/)

Проверку электронного служба хранилища Cлужбы мультимедиа microsoft *attestation* for SEC Rule 17a-4 можно запросить, создав билет поддержки с [поддержкой](https://azure.microsoft.com/support/create-ticket/) [Azure.](https://azure.microsoft.com/support/plans/) В этом письме для проверки корпорация Майкрософт предоставляет гарантии, которые помогут клиентам выполнить требования SEC 17a-4(f)(2).

### <a name="office-365--sec-rule-17"></a>Office 365 & SEC Rule 17

- [Оценка соответствия требованиям SEC 17a-4(f): Центр соответствия требованиям & microsoft Security SharePoint, OneDrive, Teams, Exchange и Skype для бизнеса](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=2dc92867-5f83-49d8-ad04-9e7295c9e40e&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_FAQ_and_White_Papers)

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

- [Документация Azure по соответствию требованиям](/azure/compliance/)
- [Обеспечение соответствия требованиям Azure](https://azure.microsoft.com/resources/azure-enables-a-world-of-compliance/)
- [Правило](https://www.sec.gov/) [17a-4](https://www.sec.gov/rules/final/34-38245.txt) Exchange комиссии по ценным бумагам и ценным бумагам
- [Ресурсы финансовых служб Microsoft Cloud](https://servicetrust.microsoft.com/viewpage/financialservicesoverview)
- [Программа соответствия требованиям к финансовым службам Microsoft Cloud](https://aka.ms/FSCP-Print)
- [Карта соответствия принципам регулирования облачных вычислений и сетевым службам Майкрософт](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides)
- [Руководство по оценке рисков и соответствия требованиям для финансовых учреждений в Microsoft Cloud](https://azure.microsoft.com/resources/risk-assessment-and-compliance-guide-for-financial-institutions-in-the-microsoft-cloud-/)
- [Случаи использования отрасли финансовых служб](/azure/industry/financial/)
- [Архивативная Microsoft Office 365, хранение данных и правило 17a-4](https://www.microsoft.com/microsoft-365/blog/2015/11/10/office-365-exchange-online-archiving-now-meets-sec-rule-17a-4-requirements/)
