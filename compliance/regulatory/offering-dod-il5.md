---
title: Уровень воздействия Министерства обороны (DoD) 5 (IL5)
description: Узнайте, как Корпорация Майкрософт отвечает стандартам Управления обороны (DoD) по уровню воздействия 5 (IL5).
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
ms.openlocfilehash: 539a53888ec859bb3b6942b48288659f73fa4b69807ce19e063cbfe104b7072d
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54294236"
---
# <a name="department-of-defense-dod-impact-level-5-il5"></a>Уровень воздействия Министерства обороны (DoD) 5 (IL5)

## <a name="dod-il5-overview"></a>Обзор DoD IL5

Агентство информационных систем обороны (DISA) — это агентство Министерства обороны США, которое отвечает за разработку и обслуживание руководства по безопасности облачных вычислений DoD [(SRG).](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html) SRG определяет базовые требования к безопасности, используемые DoD для оценки позиции безопасности поставщика облачных служб (CSP), поддерживающих решение о предоставлении предварительной авторизации (PA) DoD, которая позволяет CSP принимать миссии DoD. Он включает, заметив и отменить ранее опубликованную модель облачной безопасности DoD (CSM) и карты в Рамках управления рисками DoD (RMF).

DISA направляет агентства и отделы Министерства обороны в планировании и санкционировании использования CSP. Он также оценивает предложения CSP на соответствие SRG , процесс авторизации, в соответствии с которой CSPs может предоставлять документацию, из которой следует, что они соответствует стандартам DoD. При необходимости он выдает временные разрешения doD, поэтому агентства doD и поддерживающие организации могут использовать облачные службы без необходимости самостоятельного полного утверждения, экономя время и усилия.

В соответствии [с разделом SRG 3.2](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#3.2InformationImpactLevels) Уровни воздействия *на информацию,* информация il5 охватывает:

- Контролируемые неклассифицированные сведения (CUI), которые требуют более высокого уровня защиты, чем для IL4
    - Реестр [CUI](https://www.archives.gov/cui) предоставляет определенные категории сведений, которые находятся под защитой исполнительной ветви, например, более 20 групп категорий включены в список [категорий CUI.](https://www.archives.gov/cui/registry/category-list)
    - [NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final) *Protected Controlled Unclassified Information in Nonfederal Systems and Organisations* is intended for use by federal agencies in contracts or other agreements established with non-federal organisations.

- Системы национальной безопасности (NSS)
    - [Руководство NIST SP 800-59](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-59.pdf)  по определению информационной системы в качестве системы национальной безопасности предоставляет определения NSS.
    - [CnSSI 1253](https://www.dcsa.mil/portals/91/documents/ctp/nao/CNSSI_No1253.pdf) *Категория* безопасности и выбор управления для национальных систем безопасности предоставляют рекомендации по стандартам безопасности, которые федеральные учреждения должны применять для классификации сведений о национальной безопасности.

В памятке doD CIO от 15 декабря  [2014](https://www.esi.mil/contentview.aspx?id=585) г. о обновленных руководствах по приобретению и использованию коммерческих облачных вычислительных служб говорится, что "FedRAMP будет служить минимальным базовым уровнем безопасности для всех облачных служб DoD". SRG использует базовую линию FedRAMP Moderate на всех уровнях влияния информации (IL) и рассматривает высокий базовый уровень в некоторых случаях.

В разделе [SRG 5.1.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) DoD управления безопасностью *FedRAMP* говорится, что для оценки CSP для присвоения AD PA в IL5 используются средства управления и управления DoD FedRAMP+. Независимо от того, какой базовый уровень C/CE используется в качестве основы для high PA FedRAMP, необходимо будет оценить и утвердить дополнительные соображения и/или требования до того, как в IL5 может быть присуждена доцентка DoD PA. В частности, в разделе [SRG 5.1.2](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD FedRAMP+ Security Controls/Enhancements* в таблице 2 говорится, что для ПА DOD IL5 требуется 10 дополнительных C/CEs за пределами базового уровня FedRAMP High.

Кроме того, в соответствии с разделом [SRG 5.2.2.3](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5.2LegalConsiderations) Требования к расположению и разделению *IL5,* для pa уровня 5 должны быть следующие требования( среди прочих).

- Для этого достаточно виртуального и логического разделения между клиентами и миссиями DoD и Федеральным правительством. Требуется виртуальное и логическое разделение между системами клиента и миссии.
- Требуется физическое отделение от клиентов, не введенных в DoD/non-Federal Government (то есть клиентов государственных, местных и государственных органов).
- CSP ограничивает потенциальный доступ к данным DoD и сообщества для сотрудников CSP, которые являются гражданами США.

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Затрагиваемые облачные платформы и службы Майкрософт

- Azure
- Служба поддержки клиентов Dynamics 365
- Microsoft Defender для конечной точки (ранее Расширенная защита от угроз в Microsoft Defender)
- Microsoft Graph
- Microsoft Stream
- Office 365 для министерства обороны США
- Power Automate (прежнее название Microsoft Flow)
- Power BI

## <a name="azure-dynamics-365-and-dod-il5"></a>Azure, Dynamics 365 и DoD IL5

Дополнительные сведения о соответствии Azure, Dynamics 365 и другим сетевым службам см. в предложении [Azure DoD IL5.](/azure/compliance/offerings/offering-dod-il5)

## <a name="office-365-and-dod-il5"></a>Office 365 и DoD IL5

### <a name="office-365-cloud-environments"></a>Облачные среды Office 365

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Применимость Office 365 и затрагиваемые службы

Чтобы определить применимость служб и подписки Office 365, используйте следующую таблицу.

| **Применимость** | **Затрагиваемые службы** |
|:------------------|:----------------------|
| **DoD** | Служба каналов активности, Bing Services, Exchange Online, Exchange Online Protection, Intelligent Services, Microsoft Teams, Office 365 customer Portal, Office Online, Office Service Infrastructure, Office Use Reports, OneDrive для бизнеса, People Card, SharePoint Online, Skype для бизнеса, Windows Ink |

### <a name="attestation-documents"></a>Документы для проверки

Государственные клиенты США могут запрашивать Office 365 документацию FedRAMP для государственной обороны США непосредственно в [FedRAMP Marketplace,](https://marketplace.fedramp.gov/#!/products?sort=productName&productNameSearch=azure) подав форму запроса на доступ к пакету. Чтобы получить доступ к пакету безопасности FedRAMP непосредственно из FedRAMP, необходимо иметь адрес электронной почты .gov или .mil.

Выберите документацию FedRAMP и DoD, в том числе План системной безопасности (SSP), отчеты о непрерывном мониторинге, план действий и вехи (POA M) и т. д., доступны для клиентов в соответствии с NDA и ожидающих разрешения доступа из раздела Отчеты аудита портала доверия \& [службы - Отчеты FedRAMP.](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3) Обратитесь за помощью к представителю учетной записи Майкрософт.

### <a name="resources"></a>Ресурсы

- [Решения для правительства Майкрософт](https://www.microsoft.com/enterprise/government)
- [Руководство по обеспечению безопасности облачных вычислений DoD](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)
- [Документы FedRAMP](https://www.fedramp.gov/documents/)
- [Инструкция DoD 8510.01](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodi/851001p.pdf) *DoD Risk Management Framework (RMF)* для информационных технологий DoD (IT)
- База управления рисками для информационных систем и организаций [NIST SP 800-37:](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) системный подход Life-Cycle безопасности *и конфиденциальности*
- [NIST SP 800-53](https://csrc.nist.gov/Projects/risk-management/sp800-53-controls/release-search#!/800-53) Управление безопасностью и *конфиденциальностью для информационных систем и организаций*
- [Руководство NIST SP 800-59](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-59.pdf) по идентификации информационной *системы в качестве системы национальной безопасности*
- [CnSSI 1253](https://www.dcsa.mil/portals/91/documents/ctp/nao/CNSSI_No1253.pdf) Категория безопасности и выбор управления *для национальных систем безопасности*
- [NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final) Для защиты неклассифицированной информации в *нефедеральных* системах и организациях
- Контролируемый реестр неклассифицированных сведений (CUI) [и](https://www.archives.gov/cui) список категорий [CUI](https://www.archives.gov/cui/registry/category-list).
