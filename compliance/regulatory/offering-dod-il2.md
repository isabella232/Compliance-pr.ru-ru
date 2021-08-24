---
title: Уровень воздействия Министерства обороны (DoD) 2 (IL2)
description: Узнайте, как Корпорация Майкрософт отвечает стандартам 2 (IL2) для Министерства обороны (DoD).
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
ms.openlocfilehash: c57183a53c563fffa2bb3eb1cedb2fca23db26f4
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/23/2021
ms.locfileid: "58482452"
---
# <a name="department-of-defense-dod-impact-level-2-il2"></a>Уровень воздействия Министерства обороны (DoD) 2 (IL2)

## <a name="dod-il2-overview"></a>Обзор DoD IL2

Агентство информационных систем обороны (DISA) — это агентство Министерства обороны США, которое отвечает за разработку и обслуживание руководства по безопасности облачных вычислений DoD [(SRG).](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html) SRG определяет базовые требования к безопасности, используемые DoD для оценки позиции безопасности поставщика облачных служб (CSP), поддерживающих решение о предоставлении предварительной авторизации (PA) DoD, которая позволяет CSP принимать миссии DoD. Он включает, заметив и отменить ранее опубликованную модель облачной безопасности DoD (CSM) и карты в Рамках управления рисками DoD (RMF).

DISA направляет агентства и отделы Министерства обороны в планировании и санкционировании использования CSP. Он также оценивает предложения CSP на соответствие SRG , процесс авторизации, в соответствии с которой CSPs может предоставлять документацию, из которой следует, что они соответствует стандартам DoD. При необходимости он выдает временные разрешения doD, поэтому агентства doD и поддерживающие организации могут использовать облачные службы без необходимости самостоятельного полного утверждения, экономя время и усилия.

В памятке doD CIO от 15 декабря  [2014](https://www.esi.mil/contentview.aspx?id=585) г. о обновленных руководствах по приобретению и использованию коммерческих облачных вычислительных служб говорится, что "FedRAMP будет служить минимальным базовым уровнем безопасности для всех облачных служб DoD". SRG использует базовую линию FedRAMP Moderate на всех уровнях влияния информации (IL) и рассматривает высокий базовый уровень в некоторых случаях.

В разделе [SRG 5.1.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) DoD управления безопасностью *FedRAMP* говорится, что информация IL2 может быть организована в CSP, где минимально имеется умеренный PA FedRAMP и PA уровня DoD 2 при условии соблюдения требований безопасности персонала, изложенных в разделе 5.6.2. Однако этот подход не облегчает CSP другие требования к безопасности и интеграции, как того требует владелец миссии. Согласно [SRG Section 5.2.2.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5.2LegalConsiderations) IL2 Location *and Separation Requirements,* DOD IL2 PA адекватно покрывается pa FedRAMP Moderate, чтобы требования не были дополнительно оценены для PA IL2.

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Затрагиваемые облачные платформы и службы Майкрософт

- Azure
- Dynamics 365
- Microsoft Cloud App Security
- Microsoft Defender для конечной точки
- Microsoft Graph
- Microsoft Intune
- Microsoft Stream
- Office 365 Правительство США, Office 365 правительство США - Высокая
- Power Apps
- Power Automate
- Power BI

## <a name="azure-dynamics-365-and-dod-il2"></a>Azure, Dynamics 365 и DoD IL2

Дополнительные сведения о соответствии Azure, Dynamics 365 и другим сетевым службам см. в предложении [Azure DoD IL2.](/azure/compliance/offerings/offering-dod-il2)

## <a name="office-365-and-dod-il2"></a>Office 365 и DoD IL2

### <a name="office-365-cloud-environments"></a>Облачные среды Office 365

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Применимость Office 365 и затрагиваемые службы

Чтобы определить применимость служб и подписки Office 365, используйте следующую таблицу.

| **Применимость** | **Затрагиваемые службы** |
|:------------------|:----------------------|
| **GCC** | Служба каналов активности, службы Bing, Delve, Exchange Online Protection, Exchange Online, интеллектуальные службы, Microsoft Teams, Office 365 клиентский портал, Office Online, инфраструктура Office, Office Отчеты об использовании, OneDrive для бизнеса, Карточка людей, SharePoint Online, Skype для бизнеса, Windows Ink |
| **GCC High** | Служба каналов активности, службы Bing, Delve, Exchange Online Protection, Exchange Online, интеллектуальные службы, Microsoft Teams, Office 365 клиентский портал, Office Online, инфраструктура Office, Office Отчеты об использовании, OneDrive для бизнеса, Карточка людей, SharePoint Online, Skype для бизнеса, Windows Ink |

### <a name="resources"></a>Ресурсы

- [Решения для правительства Майкрософт](https://www.microsoft.com/enterprise/government)
- [Руководство по обеспечению безопасности облачных вычислений DoD](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)
- [Документы FedRAMP](https://www.fedramp.gov/documents/)
- База управления рисками для информационных систем и организаций [NIST SP 800-37:](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) системный подход Life-Cycle безопасности *и конфиденциальности*
- [NIST SP 800-53](https://csrc.nist.gov/Projects/risk-management/sp800-53-controls/release-search#!/800-53) Управление безопасностью и *конфиденциальностью для информационных систем и организаций*
- [Инструкция DoD 8510.01](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodi/851001p.pdf) *DoD Risk Management Framework (RMF)* для информационных технологий DoD (IT)
