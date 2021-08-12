---
title: Правило 4511 (c) США
description: Независимая компания по оценке подтвердила, что Azure и Office 365 могут помочь финансовым фирмам соответствовать требованиям к хранению записей FINRA Rule 4511 и неопровержимым требованиям к хранению.
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
ms.openlocfilehash: 0b45e9e526ad95030eed1a6b7b1814ad4aee66e8b33651ee466d71795ba97f74
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54287438"
---
# <a name="financial-industry-regulatory-authority-finra-rule-4511c-united-states"></a>Правило 4511 (c) США

## <a name="about-finra-rule-4511"></a>О правиле FINRA 4511

Управление по регулированию финансовой отрасли [(FINRA)](https://www.finra.org/#/) — это крупнейший независимый орган, регулирующий деятельность фирм с ценными бумагами, контролирующий более 4500 брокерских фирм в США. Он был санкционирован Конгрессом США "для защиты американских инвесторов, убедившись, что брокер-дилерская индустрия работает честно и честно".

В 2011 году Комиссия по безопасности и Exchange США (SEC) одобрила принятие FINRA правил SEC, регулирующих хранение книг и записей на электронных носительх хранения. [Правило FINRA 4511(c)](https://www.finra.org/sites/default/files/NoticeDocument/p123548.pdf) указывает, что "все книги и записи, которые должны быть сделаны в соответствии с правилами FINRA, должны сохраняться в формате и носитель, который соответствует правилу 17a-4 SEA (Securities Exchange Act) ".

Кроме того, правило FINRA 4511(c) требует от фирм сохранять на срок не менее шести лет те книги и записи, для которых не существует определенного периода хранения в соответствии с применимыми правилами FINRA или SEA. Фактически, если книги и записи относятся к учетной записи, срок хранения должен быть шесть лет после закрытия учетной записи. В противном случае срок хранения составляет шесть лет после создания таких книг и записей.

## <a name="microsoft-and-finra-rule-4511c"></a>Правило Microsoft и FINRA 4511(c)

Клиенты финансовых служб, представляющие одну из наиболее строго регулируемых отраслей в мире, подвержены сложным положениям, таким как хранение финансовых транзакций и связанных с ними сообщений в неустанных и неустанных состояниях. Среди них правило 4511 Органа регулирования финансовой отрасли (FINRA), которое предусматривает строгие требования к регулируемым организациям, которые выбирают для хранения книг и записей на электронных носительх хранения. Записи, хранимые, должны быть ненадеженными без возможности изменять или удалять их до окончания назначенного периода хранения.

Microsoft Azure Неизменяемые Blob служба хранилища с блокировкой политики и Microsoft Office 365 с блокировкой сохранения могут помочь финансовым учреждениям выполнить неизменяемые требования к хранению правила FINRA 4511(c).

## <a name="microsoft-azure"></a>Microsoft Azure

Чтобы оценить соответствие Azure правилу FINRA 4511(c), Корпорация Майкрософт сохранила независимую фирму по оценке, которая специализируется на управлении записями и управлении информацией, Cohasset Associates. В итоговом отчете [SEC 17a-4(f) & CFTC 1.31 (c-d)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=19b08fd4-d276-43e8-9461-715981d0ea20&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_GRC_Assessment_Reports)Оценка соответствия требованиям: служба хранилища Microsoft Azure, включает соответствие Azure правилу FINRA 4511(c), которое относя к формату и требованиям к средствам массовой информации правила SEC 17a-4(f).

Cohasset подтвердила, что [azure Immutable Blob служба хранилища](/azure/storage/blobs/storage-blob-immutable-storage) с параметром Блокировка политики, когда используется для сохранения временного Blobs в формате, не стираемом и не перезаписываемом (WORM), соответствует соответствующим требованиям хранения FINRA. Каждый Blob (запись) защищен от изменения, перезаписи или удаления, пока не истечет необходимый период хранения и не будут выпущены все связанные юридические удержания.

Поставщики программного обеспечения и партнеры с конфиденциальными рабочими нагрузками теперь могут использовать Azure Immutable Blob служба хранилища в качестве облачного решения магазина для хранения записей и неоменяемого хранения. Финансовые учреждения теперь могут создавать собственные приложения, пользуясь этими функциями, оставаясь совместимыми.

## <a name="microsoft-365"></a>Microsoft 365

Для требований правила [FINRA 4511(c)](/microsoft-365/compliance/retention-regulatory-requirements#sec-17a-4f-finra-4511c-and-cftc-131c-d) Cohasset подтвердил, что Microsoft 365 включает функции архивации, которые позволяют регулируемым клиентам, включая брокеров-дилеров, хранить данные таким образом, чтобы они могли соответствовать требованиям SEC для хранения записей. Функции хранения Microsoft 365 сохраняют широкий спектр данных, включая электронную почту, голосовую почту, общие документы, мгновенные сообщения и сторонние данные. В частности, архивирование в Microsoft 365 позволяет клиентам устанавливать глобальные или гранулярные политики хранения сообщений для хранения данных за определенный период и за его пределами в неописуемом, не стираемом формате.

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Затрагиваемые облачные платформы и службы Майкрософт

- [Azure](https://gallery.technet.microsoft.com/Overview-of-Azure-c1be3942)
- [Office 365](https://aka.ms/Office365ComplianceOfferings)

## <a name="audits-reports-and-certificates"></a>Аудит, отчеты и сертификаты

### <a name="azure--finra-rule-4511c"></a>Azure & FINRA Rule 4511(c)

[Sec 17a-4(f) & CFTC 1.31 (c-d) Оценка соответствия требованиям служба хранилища Azure](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=19b08fd4-d276-43e8-9461-715981d0ea20&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_GRC_Assessment_Reports)

### <a name="office-365--finra-rule-4511c"></a>Office 365 & FINRA Rule 4511(c)

[Архивка в Office 365, хранение данных и соответствие правилу SEC 17a-4](https://www.microsoft.com/microsoft-365/blog/2015/11/10/office-365-exchange-online-archiving-now-meets-sec-rule-17a-4-requirements/)

## <a name="how-to-implement"></a>Методика реализации

- **Регулирование финансовых служб:** карта соответствия ключевым принципам регулирования США для облачных вычислений и онлайн-служб Microsoft. [Подробнее](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides)
- **Руководство по оценке риска и соответствия требованиям**. Создание модели управления для оценки рисков облачных служб Майкрософт и уведомления контролирующих органов. [Подробнее](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=edee9b14-3661-4a16-ba83-c35caf672bd7&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_FAQ_and_White_Papers)
- **Финансовые варианты использования**. Обзоры вариантов использования, учебные руководства и другие ресурсы для создания решений Azure для сферы финансовых услуг. [Подробнее](/azure/industry/financial/)

## <a name="resources"></a>Ресурсы

- [Программа соответствия финансовых услуг Microsoft Financial Services Compliance Program](https://download.microsoft.com/download/6/4/7/64707E3E-6D3E-45D0-8207-A0EA3201B4A6/Microsoft%20Cloud%20-%20Financial%20Services%20Compliance%20Program%20\(Print\).pdf)
- [Облачные службы Майкрософт для бизнеса и финансовые услуги](https://servicetrust.microsoft.com/viewpage/financialservicesoverview)
- [Соответствие финансовых услуг требованиям в Azure](https://azure.microsoft.com/resources/videos/azurecon-2015-financial-services-compliance-in-azure/)
- [Средство оценки облачных рисков для финансовых услуг в Azure](https://servicetrust.microsoft.com/ViewPage/FFIECBlueprint?command=Download&downloadType=Document&downloadId=079a1973-711a-428f-9312-9ddd290cff7b&docTab=c726d5c0-2d1e-11e8-a485-57140ec19669_PaaS)
- [Microsoft Office 365 Политики хранения](/office365/securitycompliance/retention-policies)
- [Блог финансовых услуг Майкрософт](https://techcommunity.microsoft.com/t5/Financial-Services-Blog/bg-p/FinancialServicesBlog)
- [Соответствие требованиям в центре управления безопасностью Майкрософт](https://www.microsoft.com/trust-center/compliance/compliance-overview)
