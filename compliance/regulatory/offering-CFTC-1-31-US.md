---
title: Правило 1.31(c-d) Комиссии по товарным рынкам США (CFTC)
description: Независимая компания по оценке проверила, что Azure и Office 365 могут помочь финансовым компаниям соответствовать правилу CFTC 1.31 по хранению записей и неуменяемым требованиям к хранилищу.
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
ms.openlocfilehash: 474cd04d98dc91668e48d1999f4fbd91d81523ec
ms.sourcegitcommit: 21ed42335efd37774ff5d17d9586d5546147241a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2021
ms.locfileid: "50121758"
---
# <a name="commodity-futures-trading-commission-cftc-rule-131c-d-united-states"></a>Правило 1.31(c-d) Комиссии по товарным рынкам США (CFTC)

## <a name="about-cftc-rule-13c-d"></a>О правиле CFTC 1.3(c-d)

Комиссия [по торговли](https://www.cftc.gov/) товарными рынками (CFTC), независимое федеральное агентство США, регулирует товарные рынки и рынки параметров, а в последнее время — рынок подкачки.  
  
Постоянное правило CFTC 1.31 определяет требования к хранению записей, установленные правилом SEC 17a-4(f). Кроме того, в нем указывается, что электронные записи должны храниться в течение пяти лет, а исходные записи должны быть доступны в течение первых двух лет и быть доступными для проверки Комиссией или министерством по надзору США в течение всего периода хранения.  
  
В 2017 г. [CFTC](https://www.cftc.gov/sites/default/files/idc/groups/public/@lrfederalregister/documents/file/2017-11014a.pdf)пересмотрел свое правило, внося изменения и модернизацию норматива регистрации, чтобы принять менее предписывающие принципы стандарты, которые обеспечивают большую гибкость в обслуживании записей. Это изменение делает правило более нейтральным с точки зрения технологий, позволяя регулируемым организациям выбирать технологию, наиболее подместимую для их бизнеса, сохраняя при этом меры безопасности, "обеспечивающие надежность процесса регистрации". Пересмотренное правило удаляет требование, чтобы организации сохраняли исходные записи в течение двух лет, но сохраняет пятилетний период обслуживания, который согласуется с практиками для компаний, регулируемых CFTC и SEC.

## <a name="microsoft-and-cftc-rule-131c-d"></a>Microsoft и правило CFTC 1.31(c-d)

Клиенты финансовых услуг, представляющие одну из наиболее жестко регулируемых отраслей в мире, подвержены сложным положениям, таким как хранение финансовых транзакций и связанных коммуникаций в неутираемом и не изумяемом состоянии. Одним из наиболее строгих требований является правило 1.31 Комиссии по торговли товарными рынками США (CFTC), которое устанавливает строгие требования для регулируемых организаций, которые выбирают хранение книг и записей на электронных носитах. Хранимые записи не должны быть изменены или удаляться до окончания указанного периода хранения. Microsoft Azure Immutable BLOB Storage with Policy Lock and Microsoft Office 365 with Preservation Lock can help financial institutions meet the storage requirements of CFTC Rule 1.31(c-d).

### <a name="microsoft-azure"></a>Microsoft Azure

Для оценки соответствия Azure правилу CFTC 1.31 (c-d) корпорация Майкрософт сохранила независимую компанию по оценке, специализирующуюся на управлении записями и управлении информацией, Cohasset Associates. В итоговом отчете [cfTC 1.31 (c)–(d) Compliance Assessment: Microsoft Azure Storage](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=19b08fd4-d276-43e8-9461-715981d0ea20&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_GRC_Assessment_Reports), Cohasset validated that [Azure Immutable BLOB Storage](/azure/storage/blobs/storage-blob-immutable-storage) with the Policy Lock option, when used to retain time-based BLOBs in a non-erasable and non-rewritable (WORM) format, meets the principles-based requirements of the CFTC rule. Каждый BLOB-проект (запись) защищен от изменения, перезаписи или удаления до истечения требуемого срока хранения и освобождения всех связанных юридических удержаний. Поставщики программного обеспечения и партнеры с конфиденциальными рабочими нагрузками теперь могут полагаться на неуявяемое хранилище BLOB-данных Azure в качестве облачного решения для однообъектного магазина для хранения записей. Финансовые учреждения теперь могут создавать собственные приложения, пользуясь преимуществами этих функций, при этом оставаясь совместимыми.

### <a name="microsoft-365"></a>Microsoft 365

В отношении требований [CFTC 1.31(c)-(d)](/microsoft-365/compliance/retention-regulatory-requirements#sec-17a-4f-finra-4511c-and-cftc-131c-d) Компания Cohasset проверила, что Microsoft 365 включает функции архивации, позволяющие регулируемым клиентам, включая брокеров-брокеров, хранить данные таким образом, чтобы они соответствовали требованиям SEC для хранения записей. Функции хранения в Microsoft 365 помогают сохранять широкий спектр данных, включая электронную почту, голосовую почту, общие документы, мгновенные сообщения и сторонние данные. В частности, архивирование в Microsoft 365 позволяет клиентам устанавливать глобальные или детализируемые политики хранения сообщений для хранения данных в течение определенного периода и более длительного периода в неопределяемом и неусвояемом формате.

## <a name="microsoft-in-scope-cloud-services"></a>Облачные службы Майкрософт, к которым применима оценка

- [Azure](https://aka.ms/AzureCompliance)
- [Office 365](https://aka.ms/o365-compliance-framework)

## <a name="audits-reports-and-certificates"></a>Аудит, отчеты и сертификаты

[Azure & ПРАВИЛО CFTC 1.31: оценка соответствия требованиям CFTC 1.31 (c-d) хранилища Azure с sec 17a-4(f) & CFTC 1.31(c-d)

[Office 365 & CFTC Rule 1.31: Archiving in Office 365, data retention, and SEC Rule 17a-4 compliance

## <a name="how-to-implement"></a>Методика реализации

- [Регулирование финансовых услуг](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides): карта соответствия основным принципам законодательства США для облачных вычислений и веб-служб Майкрософт.
- [Руководство по оценке риска и соответствия требованиям](https://aka.ms/RiskGovernanceGuide). Создание модели управления для оценки рисков облачных служб Майкрософт и уведомления контролирующих органов.
- [Финансовые варианты использования](/azure/industry/financial/). Обзоры вариантов использования, учебные руководства и другие ресурсы для создания решений Azure для сферы финансовых услуг.

## <a name="resources"></a>Ресурсы

- [Программа соответствия финансовых услуг Microsoft Financial Services Compliance Program](https://aka.ms/FSCP-Print)
- [Облачные службы Майкрософт для бизнеса и финансовые услуги](https://www.microsoft.com/trustcenter/cloudservices/financialservices)
- [Соответствие финансовых услуг требованиям в Azure](https://azure.microsoft.com/resources/videos/azurecon-2015-financial-services-compliance-in-azure/)
- [Microsoft Office 365 Retention Policies](/office365/securitycompliance/retention-policies)
- [Блог финансовых услуг Майкрософт](https://techcommunity.microsoft.com/t5/Financial-Services-Blog/bg-p/FinancialServicesBlog)
- [Соответствие требованиям в центре управления безопасностью Майкрософт](https://www.microsoft.com/trust-center/compliance/compliance-overview)
