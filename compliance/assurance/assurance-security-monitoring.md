---
title: Обзор мониторинга безопасности
description: Узнайте о мониторинге безопасности в Microsoft 365
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
hideEdit: true
ms.openlocfilehash: d0285110c3fe4225ba2e2c6d1fb58820ff2a1dc8
ms.sourcegitcommit: 07578a8e03b931f47c49f4e34b78cf8ba0605e8f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2021
ms.locfileid: "53573617"
---
# <a name="security-monitoring-overview"></a>Обзор мониторинга безопасности

## <a name="what-is-microsofts-strategy-for-monitoring-security"></a>Какова стратегия Корпорации Майкрософт по мониторингу безопасности?

Microsoft 365 постоянное наблюдение за безопасностью своих систем для обнаружения и реагирования на угрозы Microsoft 365 services. Основные принципы мониторинга безопасности и оповещения:

- Надежность: сигналы и логика для обнаружения различных действий атаки
- Точность: значимые оповещения, чтобы не отвлекаться от шума
- Скорость: возможность поймать злоумышленников достаточно быстро, чтобы остановить их

Автоматизация, масштаб и облачные решения являются ключевыми столпами нашей стратегии мониторинга и реагирования. Для эффективного отслеживания и остановки атак в масштабе некоторых Microsoft 365 основных служб нашим системам мониторинга необходимо автоматически поднимать высокоточное оповещение в режиме реального времени. Кроме того, при обнаружении проблемы нам необходима возможность уменьшить риск в масштабе, поэтому мы не можем полагаться на нашу команду, чтобы вручную устранять проблемы с помощью машины. Чтобы уменьшить риски в масштабе, мы используем облачные средства для автоматического применения контрмер и предоставления инженерам средств для быстрого применения утвержденных смягчений в среде.

## <a name="how-does-microsoft-365-perform-security-monitoring"></a>Как Microsoft 365 мониторинг безопасности?

Microsoft 365 централизованного ведения журнала для сбора и анализа событий журнала для действий, которые могут указывать на инцидент безопасности. Централизованные средства ведения журнала объединяют журналы из всех системных компонентов, включая журналы событий, журналы приложений, журналы управления доступом и системы обнаружения вторжений на основе сети. Помимо данных о журнале серверов и уровне приложений, базовая инфраструктура в нашей службе оснащена настраиваемыми агентами безопасности, которые создают подробные телеметрии и обеспечивают обнаружение вторжений на основе хостов. Эту телеметрию мы используем для мониторинга и судебной экспертизы.

Собираемые данные ведения журнала и телеметрии позволяют 24/7 оповещать о безопасности. Наша система оповещения анализирует данные журналов по мере их загрузки, выпуская оповещения в режиме реального времени. Это включает оповещения на основе правил и более сложные оповещения на основе моделей машинного обучения. Наша логика мониторинга выходит за рамки общих сценариев атак и включает глубокое понимание архитектуры и операций службы. Мы используем данные мониторинга безопасности для непрерывного улучшения наших моделей для обнаружения новых типов атак и повышения точности нашего мониторинга безопасности.

## <a name="how-does-microsoft-365-respond-to-security-monitoring-alerts"></a>Как Microsoft 365 на оповещения мониторинга безопасности?

Если нам необходимо принять меры в ответ на предупреждение или дополнительно изучить результаты судебно-медицинской экспертизы по всей службе, наши облачные средства позволяют нам быстро реагировать во всей среде. Эти средства включают полностью автоматизированные интеллектуальные агенты, которые реагируют на обнаруженные угрозы с помощью мер безопасности. Во многих случаях эти агенты развертывают автоматические контрмеры, чтобы уменьшить масштабы обнаружения безопасности без вмешательства человека. Если это невозможно, система мониторинга безопасности автоматически оповещает соответствующих дежурных инженеров, которые оснащены набором средств, позволяющих им действовать в режиме реального времени для уменьшения масштабирования обнаруженных угроз. Возможные инциденты, перенастримые в Microsoft 365 безопасности, решаются с помощью процесса реагирования на инциденты безопасности.

## <a name="how-does-microsoft-365-monitor-system-availability"></a>Как Microsoft 365 контролировать доступность системы?

Microsoft 365 активно отслеживает свои системы для показателей чрезмерного использования ресурсов и ненормального использования. Мониторинг ресурсов дополняется избыточностью служб, чтобы избежать непредвиденных простоев и обеспечить клиентам надежный доступ к продуктам и службам. Проблемы со здоровьем службы оперативно передается клиентам с помощью панели мониторинга состояния служб (SHD).

## <a name="related-external-regulations--certifications"></a>Связанные внешние правила & сертификации

Онлайн-службы Корпорации Майкрософт регулярно проверяются на соответствие внешним требованиям и сертификациям. Обратитесь к следующей таблице для проверки элементов управления, связанных с мониторингом безопасности.

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------|:--------|:------|
| [FedRAMP (Office 365)](https://compliance.microsoft.com/compliancemanager) | AC-2: управление учетной записью <br> AC-17: удаленный доступ <br> AU-7: сокращение аудита и генерация отчетов <br> SI-4: мониторинг информационной системы <br> SI-7: целостность программного обеспечения, прошивки и информации <br> | 24 сентября 2020 г. |
| [ISO 27001/27002 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> <br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.3: мониторинг доступности и планирование емкости | 20 апреля 2021 г. |
| [ISO 27017 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.3: мониторинг доступности и планирование емкости <br> A.16.1. Управление инцидентами и улучшениями информационной безопасности | 20 апреля 2021 г. |
| [SOC 1 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-19: мониторинг изменений <br> CA-26: отчет об инцидентах безопасности <br> CA-29: инженеры по вызову <br> CA-48. Журнал центра обработки данных | 24 декабря 2020 г. |
| [SOC 2 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-19: мониторинг изменений <br> CA-26: отчет об инцидентах безопасности <br> CA-29: инженеры по вызову <br> CA-30: мониторинг доступности <br> CA-48. Журнал центра обработки данных | 24 декабря 2020 г. |
| [SOC 3 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-08: сообщения об инцидентах <br> CUEC-10: контракты на обслуживание | 24 декабря 2020 г. |

## <a name="resources"></a>Ресурсы

- [За кулисами: обеспечение безопасности инфраструктуры, обеспечиваемой питанием Microsoft 365 службы](https://download.microsoft.com/download/c/4/5/c45b197e-f0d9-4f40-bd5f-ed8fc7d0cd8c/M365DCSecurityIntro_Whitepaper.pdf)
