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
ms.localizationpriority: medium
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 8ba736fbd6e72963badc3245e11cbed2292cba94
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/23/2021
ms.locfileid: "58481731"
---
# <a name="security-monitoring-overview"></a>Обзор мониторинга безопасности

## <a name="what-is-microsofts-strategy-for-monitoring-security"></a>Какова стратегия Корпорации Майкрософт по мониторингу безопасности?

Корпорация Майкрософт ведет непрерывный мониторинг безопасности своих систем для обнаружения и реагирования на угрозы сетевым службам Майкрософт. Основные принципы мониторинга безопасности и оповещения:

- Надежность: сигналы и логика для обнаружения различных действий атаки
- Точность: значимые оповещения, чтобы не отвлекаться от шума
- Скорость: возможность поймать злоумышленников достаточно быстро, чтобы остановить их

Автоматизация, масштаб и облачные решения являются ключевыми основами нашей стратегии мониторинга и реагирования. Чтобы эффективно предотвращать атаки в масштабе некоторых сетевых служб Майкрософт, нашим системам мониторинга необходимо автоматически повышать точность оповещений в режиме реального времени. Кроме того, при обнаружении проблемы нам необходима возможность уменьшить риск в масштабе, поэтому мы не можем полагаться на нашу команду, чтобы вручную устранять проблемы с помощью машины. Чтобы уменьшить риски в масштабе, мы используем облачные средства для автоматического применения контрмер и предоставления инженерам средств для быстрого применения утвержденных действий по смягчению последствий в среде.

## <a name="how-do-microsoft-online-services-perform-security-monitoring"></a>Как онлайн-службы Майкрософт выполняют мониторинг безопасности?

Веб-службы Майкрософт используют централизованные журналы для сбора и анализа событий журнала для действий, которые могут указывать на инцидент с безопасностью. Средства централизованного ведения журнала объединяют журналы из всех системных компонентов, включая журналы событий, журналы приложений, журналы управления доступом и системы обнаружения вторжений на основе сети. Помимо ведения журналов серверов и данных на уровне приложений, основная инфраструктура оснащена настраиваемыми агентами безопасности, которые создают подробные телеметрии и обеспечивают обнаружение вторжений на основе хостов. Мы используем эту телеметрию для мониторинга и экспертизы.

Собираемые данные ведения журнала и телеметрии позволяют 24/7 оповещать о безопасности. Наша система оповещений анализирует данные журнала по мере их отправки, что позволяет оповещать пользователей практически в режиме реального времени. К ним относятся оповещения на основе правил и более сложные оповещения на основе моделей машинного обучения. Наша логика мониторинга выходит за рамки общих сценариев атак и включает в себя глубокую осведомленность об архитектуре и операциях служб. Мы анализируем данные мониторинга безопасности, чтобы постоянно улучшать наши модели для обнаружения новых типов атак и повышения точности нашего мониторинга безопасности.

## <a name="how-do-microsoft-online-services-respond-to-security-monitoring-alerts"></a>Как сетевые службы Майкрософт реагируют на оповещения мониторинга безопасности?

Если события безопасности, которые вызывают оповещения, требуют принятия ответных мер или дальнейшего расследования судебно-медицинских доказательств по всей службе, наши облачные средства позволяют быстро реагировать во всей среде. К этим средствам относятся полностью автоматизированные интеллектуальные агенты, которые реагируют на обнаруженные угрозы с помощью защитных контрмер. Во многих случаях эти агенты развертывают автоматические контрмеры, чтобы масштабно уменьшить количество обнаружений в сфере безопасности без вмешательства человека. Если такой ответ невозможен, система мониторинга безопасности автоматически оповещает соответствующих дежурных инженеров, которые оснащены набором средств, позволяющих им действовать в режиме реального времени для смягчения обнаруженных угроз в масштабе. Потенциальные инциденты перенабовеяются в соответствующую команду реагирования безопасности Майкрософт и решаются с помощью процесса реагирования на инциденты безопасности.

## <a name="how-do-microsoft-online-services-monitor-system-availability"></a>Как интернет-службы Майкрософт отслеживают доступность системы?

Корпорация Майкрософт активно отслеживает свои системы для показателей чрезмерного использования ресурсов и неправильного использования. Мониторинг ресурсов дополняется избыточностью служб, чтобы избежать непредвиденных простоев и обеспечить клиентам надежный доступ к продуктам и службам. Проблемы со здоровьем веб-службы Майкрософт оперативно доносят до клиентов с помощью панели мониторинга состояния здоровья служб (SHD).

Онлайн-службы Azure и Dynamics 365 используют несколько служб инфраструктуры для мониторинга их доступности и безопасности. Реализация тестирования синтетических транзакций (STX) позволяет службам Azure и Dynamics проверять доступность своих служб. Структура STX предназначена для поддержки автоматического тестирования компонентов в запущенных службах и проверяется на оповещениях о сбое на веб-сайте в режиме live. Кроме того, служба мониторинга безопасности Azure (ASM) реализовала централизованные процедуры синтетического тестирования для проверки функции оповещений о безопасности как в новых, так и в запущенных службах.

## <a name="related-external-regulations--certifications"></a>Связанные внешние правила & сертификации

Онлайн-службы Корпорации Майкрософт регулярно проверяются на соответствие внешним требованиям и сертификациям. Обратитесь к следующей таблице для проверки элементов управления, связанных с мониторингом безопасности.

### <a name="azure-and-dynamics-365"></a>Azure и Dynamics 365

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------|:--------|:------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> <br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.3: мониторинг доступности и планирование емкости | 2 декабря 2020 г. |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.3: мониторинг доступности и планирование емкости <br> A.16.1. Управление инцидентами и улучшениями информационной безопасности | 2 декабря 2020 г. |
| [SOC 1;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | IM-1: структура управления инцидентами <br> IM-2. Конфигурация обнаружения инцидентов <br> IM-3: процедуры управления инцидентами <br> IM-4: инцидент посмертно <br> VM-1: журнал и коллекция событий безопасности <br> VM-12: мониторинг доступности служб Azure <br> VM-4: расследование вредоносных событий <br> VM-6: мониторинг уязвимости безопасности | 31 марта 2021 г. |
| [SOC 2;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | IM-1: структура управления инцидентами <br> IM-2. Конфигурация обнаружения инцидентов <br> IM-3: процедуры управления инцидентами <br> IM-4: инцидент посмертно <br> PI-2: обзор производительности портала Azure <br> VM-1: журнал и коллекция событий безопасности <br> VM-12: мониторинг доступности служб Azure <br> VM-4: расследование вредоносных событий <br> VM-6: мониторинг уязвимости безопасности | 31 марта 2021 г. |

### <a name="office-365"></a>Office 365

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------|:--------|:------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | AC-2: управление учетной записью <br> AC-17: удаленный доступ <br> AU-7: сокращение аудита и генерация отчетов <br> SI-4: мониторинг информационной системы <br> SI-7: целостность программного обеспечения, прошивки и информации <br> | 24 сентября 2020 г. |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> <br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.1.3: мониторинг доступности и планирование емкости | 20 апреля 2021 г. |
| [SOC 1;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-19: мониторинг изменений <br> CA-26: отчет об инцидентах безопасности <br> CA-29: инженеры по вызову <br> CA-48. Журнал центра обработки данных | 24 декабря 2020 г. |
| [SOC 2;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-19: мониторинг изменений <br> CA-26: отчет об инцидентах безопасности <br> CA-29: инженеры по вызову <br> CA-30: мониторинг доступности <br> CA-48. Журнал центра обработки данных | 24 декабря 2020 г. |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-08: сообщения об инцидентах <br> CUEC-10: контракты на обслуживание | 24 декабря 2020 г. |

## <a name="resources"></a>Ресурсы

- [За кадром: защита инфраструктуры, на основе которой работает служба Microsoft 365](https://download.microsoft.com/download/c/4/5/c45b197e-f0d9-4f40-bd5f-ed8fc7d0cd8c/M365DCSecurityIntro_Whitepaper.pdf)
