---
title: Правило 4511(c) для органов регулирования финансовой отрасли (FINRA) США
description: Независимая компания по оценке проверила, что Azure и Office 365 могут помочь финансовым компаниям соответствовать правилу FINRA 4511.
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
ms.openlocfilehash: f4a26a88ca742178d894b5e46d0372d91babba66
ms.sourcegitcommit: 21ed42335efd37774ff5d17d9586d5546147241a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2021
ms.locfileid: "50120848"
---
# <a name="financial-industry-regulatory-authority-finra-rule-4511c-united-states"></a>Правило 4511(c) для органов регулирования финансовой отрасли (FINRA) США

## <a name="about-finra-rule-4511"></a>О правиле FINRA 4511

Орган по надзору за финансовой отрасли [(FINRA)](https://www.finra.org/#/) — это самая большая независимая организация, регулирующая ценные бумаги, под надзором более 4500 брокерских компаний в США. Она была авториизовирована регалией США "для защиты сша от инвестиций, убедившись в том, что брокер-брокер-брокер работает относительно и добросовестно".

В 2011 г. Комиссия по безопасности и exchange (SEC) США (SEC) утверждена принятие FINRA правил SEC, управляющих хранением книг и записей на электронных носитах. Правило [FINRA 4511(c)](https://www.finra.org/sites/default/files/NoticeDocument/p123548.pdf) указывает, что "все книги и записи, необходимые для работы в соответствии с правилами FINRA, должны сохраняться в формате и носителе, который соответствует правилу 17a-4 SEA (Закона о ценных бумагах).

Кроме того, правило FINRA 4511(c) требует, чтобы компании хранили книги и записи в течение не менее шести лет, для которых не задан период хранения в соответствии с применимыми правилами FINRA или SEA. Фактически, если книги и записи относятся к учетной записи, срок хранения должен быть шесть лет после закрытия учетной записи. В противном случае срок хранения составляет шесть лет после создания таких книг и записей.

## <a name="microsoft-and-finra-rule-4511c"></a>Правило Майкрософт и FINRA 4511(c)

Клиенты финансовых услуг, представляющие одну из наиболее жестко регулируемых отраслей в мире, подвержены сложным положениям, таким как хранение финансовых транзакций и связанных коммуникаций в неутираемом и не изумяемом состоянии. Среди них — правило 4511 Надзорного органа финансовой отрасли (FINRA), которое устанавливает строгие требования для регулируемых организаций, которые выбирают хранение книг и записей на электронных носитах. Хранимые записи не должны быть изменены или удаляться до окончания указанного периода хранения.

Microsoft Azure Immutable BLOB Storage with Policy Lock and Microsoft Office 365 with Preservation Lock can help financial institutions meet the immutable storage requirements of FINRA Rule 4511(c).

## <a name="microsoft-azure"></a>Microsoft Azure

Для оценки соответствия Azure правилу FINRA 4511(c) корпорация Майкрософт сохранила независимую компанию по оценке, специализирующуюся на управлении записями и управлении информацией, Cohasset Associates. В итоговом отчете sec [17a-4(f) & CFTC 1.31 (c-d)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=19b08fd4-d276-43e8-9461-715981d0ea20&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_GRC_Assessment_Reports)о соответствии требованиям: хранилище Microsoft Azure включает соответствие Azure правилу FINRA 4511(c), которое откладывает требования к формату и носителей правила SEC 17a-4(f).

Компания Cohasset проверила, что неперемежаемые хранилища [BLOB-данных Azure](/azure/storage/blobs/storage-blob-immutable-storage) с параметром блокировки политики, если они используются для хранения BLOB-хранилищ с учетом времени в неперетираемом и неперезаписаемом формате (WORM), соответствуют соответствующим требованиям FINRA к хранилищу. Каждый BLOB-проект (запись) защищен от изменения, перезаписи или удаления до истечения требуемого срока хранения и освобождения всех связанных юридических удержаний.

Поставщики программного обеспечения и партнеры с конфиденциальными рабочими нагрузками теперь могут использовать неуменимое хранилище BLOB-хранилищ Azure в качестве облачного решения для хранения записей и неуменяемого хранилища. Финансовые учреждения теперь могут создавать собственные приложения, пользуясь преимуществами этих функций, при этом оставаясь совместимыми.

## <a name="microsoft-365"></a>Microsoft 365

В отношении требований правила [FINRA 4511(c)](/microsoft-365/compliance/retention-regulatory-requirements#sec-17a-4f-finra-4511c-and-cftc-131c-d) Компания Cohasset проверила, что Microsoft 365 включает функции архивации, позволяющие регулируемым клиентам, включая брокеров-брокеров, хранить данные таким образом, чтобы они соответствовали требованиям SEC для хранения записей. Функции хранения в Microsoft 365 помогают сохранять широкий спектр данных, включая электронную почту, голосовую почту, общие документы, мгновенные сообщения и сторонние данные. В частности, архивирование в Microsoft 365 позволяет клиентам устанавливать глобальные или детализируемые политики хранения сообщений для хранения данных в течение определенного периода и более длительного периода в неопределяемом и неусвояемом формате.

## <a name="microsoft-in-scope-cloud-services"></a>Облачные службы Майкрософт, к которым применима оценка

- [Azure](https://gallery.technet.microsoft.com/Overview-of-Azure-c1be3942)
- [Office 365](https://aka.ms/Office365ComplianceOfferings)

## <a name="audits-reports-and-certificates"></a>Аудит, отчеты и сертификаты

### <a name="azure--finra-rule-4511c"></a>Azure & FINRA Rule 4511(c)

[SEC 17a-4(f) & CFTC 1.31 (c-d) Compliance Assessment of Azure Storage](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=19b08fd4-d276-43e8-9461-715981d0ea20&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_GRC_Assessment_Reports)

### <a name="office-365--finra-rule-4511c"></a>Office 365 & FINRA Rule 4511(c)

[Архив в Office 365, хранение данных и соответствие правилу SEC 17a-4](https://www.microsoft.com/microsoft-365/blog/2015/11/10/office-365-exchange-online-archiving-now-meets-sec-rule-17a-4-requirements/)

## <a name="how-to-implement"></a>Методика реализации

- **Регулирование финансовых услуг:** карта соответствия основным принципам законодательства США для облачных вычислений и веб-служб Майкрософт. [Подробнее](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides)
- **Руководство по оценке риска и соответствия требованиям**. Создание модели управления для оценки рисков облачных служб Майкрософт и уведомления контролирующих органов. [Подробнее](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=edee9b14-3661-4a16-ba83-c35caf672bd7&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_FAQ_and_White_Papers)
- **Финансовые варианты использования**. Обзоры вариантов использования, учебные руководства и другие ресурсы для создания решений Azure для сферы финансовых услуг. [Подробнее](/azure/industry/financial/)

## <a name="resources"></a>Ресурсы

- [Программа соответствия финансовых услуг Microsoft Financial Services Compliance Program](https://download.microsoft.com/download/6/4/7/64707E3E-6D3E-45D0-8207-A0EA3201B4A6/Microsoft%20Cloud%20-%20Financial%20Services%20Compliance%20Program%20\(Print\).pdf)
- [Облачные службы Майкрософт для бизнеса и финансовые услуги](https://servicetrust.microsoft.com/viewpage/financialservicesoverview)
- [Соответствие финансовых услуг требованиям в Azure](https://azure.microsoft.com/resources/videos/azurecon-2015-financial-services-compliance-in-azure/)
- [Средство оценки облачных рисков для финансовых услуг в Azure](https://servicetrust.microsoft.com/ViewPage/FFIECBlueprint?command=Download&downloadType=Document&downloadId=079a1973-711a-428f-9312-9ddd290cff7b&docTab=c726d5c0-2d1e-11e8-a485-57140ec19669_PaaS)
- [Microsoft Office 365 Retention Policies](/office365/securitycompliance/retention-policies)
- [Блог финансовых услуг Майкрософт](https://techcommunity.microsoft.com/t5/Financial-Services-Blog/bg-p/FinancialServicesBlog)
- [Соответствие требованиям в центре управления безопасностью Майкрософт](https://www.microsoft.com/trust-center/compliance/compliance-overview)
