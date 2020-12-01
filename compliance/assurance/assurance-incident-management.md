---
title: Обзор управления инцидентами
description: Сведения об управлении инцидентами в Microsoft 365
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: article
f1.keywords:
- NOCSH
ms.service: O365-seccomp
localization_priority: Normal
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: 6b5c77a2a81f8231ad620fbc40205457c6ba1a49
ms.sourcegitcommit: 626b0076d133e588cd28598c149a7f272fc18bae
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2020
ms.locfileid: "49507851"
---
# <a name="incident-management-overview"></a>Обзор управления инцидентами

## <a name="what-is-a-security-incident"></a>Что такое инцидент безопасности?

Корпорация Майкрософт определяет инцидент безопасности в веб-службах в качестве подтвержденного нарушения безопасности, приводящего к случайному или незаконномуу уничтожению, потере, изменения, несанкционированному раскрытию или доступу к данным клиента или персональным данным при обработке корпорацией Майкрософт. Например, несанкционированный доступ к инфраструктуре Microsoft 365 и ексфилтратион данных клиентов может создать инцидент безопасности, в то время как события соответствия, которые не влияют на конфиденциальность, целостность или доступность служб или данных клиентов, не считаются инцидентами безопасности.

## <a name="how-does-microsoft-respond-to-security-incidents"></a>Как корпорация Майкрософт реагирует на инциденты безопасности?

При наличии инцидента безопасности корпорация Майкрософт стремится быстро и эффективно реагировать на защиту служб Майкрософт и данных клиентов. Корпорация Майкрософт применяет стратегию реагирования на инциденты, предназначенную для быстрого и эффективного изучения, хранения и удаления угроз безопасности.

В облачных службах Майкрософт постоянно отслеживаются признаки компромиссов. В дополнение к автоматическому мониторингу безопасности и отслеживанию оповещений все сотрудники получают ежегодное обучение для распознавания и создания отчетов о потенциальных инцидентах безопасности. Любые подозрительные действия, обнаруженные сотрудниками, клиентами или средствами мониторинга безопасности, расширяются на команды ответа безопасности, зависящие от служб, для изучения. Все Teams Operations Teams, включая зависящие от службы команды безопасности, обеспечивают глубокий цикл по вызовам, чтобы обеспечить доступность ресурсов для 24x7x365 отклика инцидентов. Наши циклы по вызовам позволяют корпорации Майкрософт подключать эффективный отклик инцидента в любое время или масштаб, в том числе распространенные или параллельные события.

Если подозрительные действия обнаружены и переданы, специалисты по безопасности, зависящие от служб, инициируют процесс **анализа, хранения, ерадикатион и восстановления**. Эти Teams выполняют анализ потенциальных инцидентов, чтобы определить его область, в том числе любое влияние на клиентов или данные клиентов. На основе этого анализа Teams, зависящие от служб, работают с затронутыми службами Teams для разработки плана, содержащего угрозу и уменьшая влияние инцидента, ерадикате угрозу из среды и полностью восстанавливая состояние безопасного состояния. Важные службы Teams реализуют план с поддержкой групп ответа на зависимые службы, чтобы убедиться в том, что угроза успешно удалена и подвержена воздействию незавершенных служб.

После устранения инцидента службы Teams реализуют все уроки, полученные из инцидента, чтобы лучше предотвратить, обнаруживать и отвечать на подобные инциденты в будущем. Выберите пункты "происшествия безопасности", особенно те, которые влияют на клиента или приведут к нарушениям данных, подвергнутые полному инциденту после аварийного происшествия. POST-дамп предназначен для определения технических промежутков, процедурных сбоев, ручных ошибок и других изъянов процесса, которые могут воздействовали на инцидент или которые были идентифицированы в процессе реагирования на инциденты. Улучшения, выявленные во время выполнения процедуры POST, реализованы с помощью координации действий, относящихся к определенным службам, чтобы предотвратить будущие происшествия и улучшить обнаружение и реагирование.

## <a name="how-and-when-are-customers-notified-of-security-or-privacy-incidents"></a>Как и когда клиенты получают уведомление о безопасности или инцидентах конфиденциальности?

Если корпорации Майкрософт известно о нарушениях безопасности, связанных с несанкционированным убытком, раскрытием или изменением данных клиента, корпорация Майкрософт уведомляет соответствующих клиентов в течение 72 часов, как описано в дополнение к защите данных (DPA) терминов Интернет-служб (OST). Заобязательство временной шкалы уведомлений начинается при возникновении официального объявления о происшествии безопасности. При объявлении инцидента безопасности процесс уведомления выполняется как можно експедитиаусли, без задержки неоправданной.

Уведомления включают описание характера нарушений, приблизительных последствий пользователей и действий по устранению рисков (если это необходимо). Если исследование на момент начального уведомления не завершено, в уведомлении также указываются следующие этапы и временные шкалы для последующего обмена данными.

Если клиент узнает об инциденте, который может оказать влияние на работу Майкрософт, в том числе на нарушение безопасности данных, клиент несет ответственность за своевременное уведомление Майкрософт об инциденте, определенном в DPA.

## <a name="related-external-regulations--certifications"></a>Связанные внешние нормативные & сертификации

Веб-службы корпорации Майкрософт регулярно подлежат аудиту для соответствия внешним нормативам и сертификациям. В следующей таблице приведены сведения о проверке элементов управления, связанных с управлением инцидентами.

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365)](https://compliance.microsoft.com/compliancemanager) | IR-4: обработка инцидентов <br> IR-6: отчеты об инцидентах <br> IR-8: план реагирования на инциденты | 24 сентября 2020 г. |
| [ISO 27001/27002 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Отчет о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A. 16.1: Управление происшествиями информационной безопасности и улучшениями | 22 февраля 2020 г. |
| [ISO 27017 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Отчет о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A. 16.1: Управление происшествиями информационной безопасности и улучшениями | 22 февраля 2020 г. |
| [ISO 27018 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Отчет о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=43e89534-f48d-42ea-a7a7-3523ff516036&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A. 10.1: уведомление о нарушении безопасности данных, связанных с PII  | 22 февраля 2020 г. |
| [SOC 1 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b07c0f7b-6bd5-4544-8255-7a5f14bf914a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Reports) | CA – 26: отчеты об инцидентах безопасности <br> CA — 47: реагирование на инциденты | 30 сентября 2019 г. |
| [SOC 2 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=fa062990-e758-4ddc-ace3-7fb21a301d09&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Rep-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Reports) | CA-12: соглашения об уровне обслуживания (SLA) <br> CA – 13: руководства по реагированию на инциденты <br> CA — 15: уведомления о работоспособности службы  <br>  <br> CA – 26: отчеты об инцидентах безопасности <br> CA — 29: инженеры по вызову <br> CA — 47: реагирование на инциденты | 30 сентября 2019 г. |
| [SOC 3 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=9df8b99b-96ce-49a9-bff4-268031dcc9a6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Reports) | КУЕК – 08: отчеты об инцидентах  | 30 сентября 2019 г.  |

## <a name="resources"></a>Ресурсы

- [Условия использования веб-служб (OST)](https://www.microsoft.com/licensing/product-licensing/products)
- [Дополнение к защите данных (DPA)](https://www.microsoft.com/licensing/product-licensing/products)
- [Руководство по внедрению управления облачными инцидентами Майкрософт для Azure и Office 365](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=a8a7cb87-9710-4d09-8748-0835b6754e95&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_FAQ_and_White_Papers)
- [Office 365 — Оценка уязвимости стороннего производителя для Office 365 — 2019](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=e85e478f-2491-435d-9c1b-2f0ad7ca8e56&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_Pen_Test_and_Security_Assessments)
