---
title: Соображения безопасности и конфиденциальности облачных вычислений правительства Новой Зеландии
description: Корпорация Майкрософт NZ решает вопросы, опубликованные в платформе облачных вычислений Новой Зеландии.
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
ms.openlocfilehash: c333fc2d6bdb9889dafefd2571b8381edd15e5158a4783aa7a17cec7ce1bcc7c
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54293386"
---
# <a name="new-zealand-government-information-security-and-privacy-considerations-ispc"></a>Сведения о безопасности и конфиденциальности правительства Новой Зеландии (ISPC)

## <a name="new-zealand-government-information-security-and-privacy-considerations-overview"></a>Обзор сведений о безопасности и конфиденциальности правительства Новой Зеландии

В октябре 2015 г. правительство Новой Зеландии одобрило пересмотренную всеуголную стратегию ИКТ, которая подтвердила свою политику "сначала облака" по использованию информационных технологий в государственном секторе. В пересмотренной стратегии сохраняется "База рисков и гарантий облачных вычислений", которая была разработана и реализована под руководством главного информационного директора правительства Новой Зеландии (GCIO).

Правительство ожидает, что все государственные службы Новой Зеландии будут работать в этом рамках при оценке и принятии облачных служб. В "Требованиях к облачным вычислениям" описывается, что должны делать агентства при принятии облачных служб, а также обзор истории облачной политики правительства.

Чтобы помочь правительственным учреждениям NZ в проведении последовательной и надежной должной осмотрительности потенциальных облачных решений, GCIO опубликовала cloud [Computing: Information Security and Privacy Considerations (ISPC).](https://www.digital.govt.nz/dmsdocument/1~cloud-computing-information-security-and-privacy-considerations/html) В этом документе содержится более 100 вопросов, которые посвящены суверенитету данных, конфиденциальности, безопасности, управлению, конфиденциальности, целостности данных, доступности и реагированию на инциденты и управлению ими. IsPC не определяет правительственный стандарт NZ, в соответствии с которым поставщики облачных служб должны демонстрировать формальное соответствие требованиям. Однако многие из вопросов, задамые в документе, указывают на важность понимания соответствия поставщиков облачных служб широкому спектру соответствующих стандартов.

## <a name="microsoft-and-new-zealand-government-cloud-computing-security-and-privacy-considerations"></a>Соображения безопасности и конфиденциальности облачных вычислений корпорации Майкрософт и Правительства Новой Зеландии

Чтобы помочь учреждениям в анализе и оценке облачных служб Майкрософт, Корпорация Майкрософт в Новой Зеландии подготовила документы, показывающие, как корпоративные облачные службы отвечают на вопросы, задающиеся в ISPC облачных вычислений, связывая их со стандартами, с которыми сертифицированы облачные службы Майкрософт. Эти сертификаты имеют центральное значение для того, как Корпорация Майкрософт гарантирует клиентам государственного и частного сектора, что ее облачные службы разработаны, построены и работают для эффективного снижения рисков конфиденциальности и безопасности и решения проблем, связанных с суверенитетом данных. Для скачивания пользователям доступен ответ Azure на [ISPC](https://azure.microsoft.com/resources/microsoft-azure-response-to-nz-gcio-cloud-computing-information-security-privacy-considerations/) облачных вычислений.

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Затрагиваемые облачные платформы и службы Майкрософт

- Azure и Azure для государственных организаций
- [Dynamics 365](https://aka.ms/d365-compliance-list)
- Intune
- Office 365
- Облачная служба Power BI в виде автономной службы или в составе плана либо набора Office 365

## <a name="office-365-and-ispc"></a>Office 365 и ISPC

### <a name="office-365-cloud-environments"></a>Облачные среды Office 365

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Применимость Office 365 и затрагиваемые службы

Чтобы определить применимость служб и подписки Office 365, используйте следующую таблицу.

| **Применимость** | **Затрагиваемые службы** |
|:------------------|:----------------------|
| **Office 365** | Exchange Online, SharePoint Online, Skype для бизнеса |

>[!Note]
>Корпорация Майкрософт NZ работала с командой GCIO над разработкой архитектуры ссылок для интеграции Exchange Online и SEEMail, описанных в Office 365: seeMail Integration and Reference Architecture.

## <a name="frequently-asked-questions"></a>Вопросы и ответы

**К кому применяется эта структура?**

Организации, подпадающие под мандат GCIO, государственные и негосударственные службы, 20 окружных советов здравоохранения и 7 субъектов Короны, должны придерживаться этой структуры при принятии решения об использовании облачной службы.

**Может ли мое агентство использовать ответы Корпорации Майкрософт на эти рамки в процессе сертификации наших систем ИКТ?**

Если ваше агентство обязано проводить сертификацию и аккредитацию своей системы ИКТ в руководстве по информационной безопасности Новой [Зеландии,](https://go.microsoft.com/fwlink/p/?linkid=2099496)вы можете использовать эти ответы в рамках анализа.

## <a name="resources"></a>Ресурсы

- [Требования к безопасности для офшорных служб Office производительности: руководство по соответствунию для Office 365](https://aka.ms/o365-gcio-conformance-guidance)
- [Стратегия ИКТ правительства NZ 2015](https://www.ict.govt.nz/strategy-and-action-plan/strategy/)
- [Облачные вычисления: соображения информационной безопасности и конфиденциальности (ISPC)](https://www.digital.govt.nz/standards-and-guidance/technology-and-architecture/cloud-services/)
- [Условия использования веб-служб Майкрософт](https://aka.ms/Online-Services-Terms)
- [Соответствие требованиям в центре управления безопасностью Майкрософт](https://www.microsoft.com/trust-center/compliance/compliance-overview)

## <a name="microsoft-responses-to-cloud-computing-ipsc"></a>Ответы Корпорации Майкрософт на IPSC облачных вычислений

- [Azure](https://aka.ms/Azure-NZ-response)
- [Intune](https://aka.ms/Intune-NZ-response)
- [Office 365](https://aka.ms/O365-NZ-Response)
- [Power BI](https://download.microsoft.com/download/5/1/7/51726B9B-2E76-49C4-9D4F-A36BF025CB93/Response-to-GCIO-105-questions-Power-BI.pdf)
