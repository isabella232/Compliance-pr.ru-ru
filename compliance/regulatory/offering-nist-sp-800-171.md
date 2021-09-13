---
title: NIST SP 800-171
description: Облачные службы Майкрософт соответствуют рекомендациям NIST SP 800-171 по защите контролируемых неклассифицированных сведений (CUI) в нефедеральных информационных системах.
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
ms.openlocfilehash: bce6847fe4c0cd1541348b70aadacc9c13238c31
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59160547"
---
# <a name="nist-sp-800-171"></a>NIST SP 800-171

## <a name="about-nist-sp-800-171"></a>О NIST SP 800-171

Национальный институт стандартов и технологий США (NIST) продвигает и поддерживает стандарты и рекомендации по измерению для защиты информационных и информационных систем федеральных учреждений. В ответ на исполнительный приказ 13556 по управлению контролируемой неклассифицированной информацией (CUI), он опубликовал [NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-1/final) *,* защита контролируемых неклассифицированных сведений в нефедеральных информационных системах и организациях . CUI определяется как сведения, как цифровые, так и физические, созданные правительством (или субъектом от его имени), которые, хотя и не классифицируются, по-прежнему являются конфиденциальными и требуют защиты.

NIST SP 800-171 был первоначально опубликован в июне 2015 г. и с тех пор несколько раз обновлялся в ответ на развитие киберугроз. В нем содержится руководство по обеспечению безопасного доступа, передачи и хранения cuI в нефедеральных информационных системах и организациях; его требования подпадают под четыре основные категории:

- Управление и процессы управления и защиты
- Мониторинг и управление ИТ-системами
- Четкие методы и процедуры для конечных пользователей
- Реализация мер технической и физической безопасности

## <a name="microsoft-and-nist-sp-800-171"></a>Microsoft и NIST SP 800-171

Аккредитованные сторонние организации оценки Kratos Secureinfo и Coalfire в партнерстве с Корпорацией Майкрософт подтвердили, что ее облачные службы соответствуют критериям nIST SP 800-171, защищая неклассифицированную неклассифицированную информацию *(CUI)* в нефедеральных информационных системах и организациях, при обработке CUI. Реализация Microsoft требований [FedRAMP](offering-fedramp.md) помогает обеспечить выполнение или превышение требований облачных служб Майкрософт к NIST SP 800-171 с помощью уже внедренных систем и методов.

Требования NIST SP 800-171 являются подмножество NIST SP 800-53, стандарта, который использует FedRAMP. Приложение D NIST SP 800-171 обеспечивает прямое сопоставление требований безопасности CUI к соответствующим средствам управления безопасностью в NIST SP 800-53, для которых облачные службы в области уже были оценены и разрешены в рамках программы FedRAMP.

Любая организация, которая обрабатывает или хранит государственные cuI США — исследовательские учреждения, консалтинговые компании, производственные подрядчики, должна соответствовать строгим требованиям NIST SP 800-171. Это подтверждение означает, что облачные службы Майкрософт могут размещать клиентов, желающих развернуть рабочие нагрузки CUI, с гарантией полного соответствия требованиям Корпорации Майкрософт. Например, все подрядчики DoD, которые обрабатывает, хранит или передает "закрытые сведения о защите", используя облачные службы Microsoft в своих информационных системах, соответствуют положениям Министерства обороны США, которые требуют соблюдения требований безопасности NIST SP 800-171.

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Затрагиваемые облачные платформы и службы Майкрософт

- Azure Commercial, Azure Government
- Dynamics 365 Правительство США
- Intune
- Office 365 U.S. облако сообщества для государственных организаций (GCC), Office 365 GCC High и DoD

## <a name="azure-dynamics-365-and-nist-sp-800-171"></a>Azure, Dynamics 365 и NIST SP 800-171

Дополнительные сведения о соответствии Azure, Dynamics 365 и другим сетевым службам см. в предложении [Azure NIST SP 800-171.](/azure/compliance/offerings/offering-nist-800-171)

## <a name="office-365-and-nist-sp-800-171"></a>Office 365 и NIST SP 800-171

### <a name="office-365-cloud-environments"></a>Облачные среды Office 365

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Применимость Office 365 и затрагиваемые службы

Чтобы определить применимость изменений к вашим службам и подписке Office 365, воспользуйтесь следующей таблицей.

| **Применимость** | **Затрагиваемые службы** |
|:------------------|:----------------------|
| **GCC** | Служба каналов активности, Bing services, Delve, Exchange Online, Intelligent Services, Microsoft Teams, Office 365 customer Portal, Office Online, Office Service Infrastructure, Office Use Reports, OneDrive для бизнеса, people Card, SharePoint Online, Skype для бизнеса, Windows Ink |
| **GCC High** | Служба каналов активности, Bing службы, Exchange Online, интеллектуальные службы, Microsoft Teams, Office 365 портал клиентов, Office Online, инфраструктура Office, Office Отчеты об использовании, OneDrive для бизнеса, Карточка людей, 
SharePoint Онлайн, Skype для бизнеса, Windows Ink |
| **DoD** | Служба каналов активности, Bing services, Exchange Online, intelligent Services, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Use Reports, OneDrive для бизнеса, People Card, Microsoft Teams, SharePoint Online, Skype для бизнеса, Windows Ink |

### <a name="frequently-asked-questions"></a>Вопросы и ответы

**Могу ли я использовать соответствие Корпорации Майкрософт NIST SP 800-171 для своей организации?**

Да. Клиенты Майкрософт могут использовать проверенные элементы управления, описанные в отчетах независимых сторонних организаций оценки (3PAO) по стандартам FedRAMP в рамках собственных усилий по анализу рисков FedRAMP и NIST. Эти отчеты свидетельствуют об эффективности элементов управления, реализованных Корпорацией Майкрософт в своих облачных службах. Клиенты несут ответственность за обеспечение соответствия рабочих нагрузок CUI требованиям NIST SP 800-171.

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>Оценка риска с помощью диспетчера соответствия требованиям (Майкрософт)

[Диспетчер соответствия требованиям (Майкрософт)](/microsoft-365/compliance/compliance-manager) — это предварительная функция в [Центре соответствия требованиям Microsoft 365](/microsoft-365/compliance/microsoft-365-compliance-center), помогающая понять состояние вашей организации в отношении соответствия требованиям и принять меры по снижению рисков. Диспетчер соответствия требованиям предоставляет премиум-шаблон для оценки этих нормативных требований. Шаблон находится на странице **шаблонов оценки** в диспетчере соответствия требованиям. См. [Создание оценки в диспетчере соответствия требованиям](/microsoft-365/compliance/compliance-manager-assessments).

### <a name="resources"></a>Ресурсы

- [Сертификация Microsoft DoD отвечает требованиям NIST 800-171](offering-DoD-DISA-L2-L4-L5.md)
- [Соответствие требованиям NIST 800-171 начинается с документации по кибербезопасности](https://www.nist800171.com/)
- [Microsoft Cloud Services FedRAMP Authorizations](https://marketplace.fedramp.gov/index.html?status=Compliant&sort=productName#/products)
- [NIST 800-171 3.3 Аудит и подотчетность с Office 365 GCC high](https://info.summit7systems.com/blog/nist-3.3-audit-and-accountability-with-office-365)
- [Microsoft и NIST Cybersecurity Framework](offering-nist-csf.md)
- [Облако Майкрософт для государственных организаций](https://www.microsoft.com/enterprise/government)
- [Соответствие требованиям в центре управления безопасностью Майкрософт](https://www.microsoft.com/trust-center/compliance/compliance-overview)
