---
title: Устойчивость и непрерывность
description: Узнайте о устойчивости и непрерывности в Microsoft 365
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
ms.openlocfilehash: ff1719ce931a50904fb6b7e6069cd29a1883aa90
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2021
ms.locfileid: "58947410"
---
# <a name="resiliency-and-continuity-overview"></a>Обзор устойчивости и непрерывности

## <a name="how-does-microsoft-ensure-business-continuity-if-a-disaster-or-other-threat-to-service-availability-occurs"></a>Как Корпорация Майкрософт обеспечивает непрерывность бизнеса в случае возникновения аварийной ситуации или другой угрозы доступности службы?

Команда управления непрерывности Enterprise бизнеса (EBCM) Корпорации Майкрософт осуществляет надзор за управлением непрерывности бизнеса и действиями по восстановлению аварийности во всех службы Майкрософт и облачных предложениях. Представители бизнес-подразделений Майкрософт координируют работу с командой EBCM для разработки планов непрерывности бизнеса и проверки соответствия требованиям непрерывности бизнеса.

Жизненный цикл управления непрерывности бизнеса (BCM) является основой нашей методологии BCM. Этот трех этапный процесс предназначен для адаптации, поэтому его можно реализовать с помощью широкого спектра бизнес-моделей корпорации Майкрософт. Она начинается с этапа **оценки** для определения критически важных процессов и задач, которые должны быть включены в программу непрерывности бизнеса. На этапе оценки также требуется анализ влияния бизнеса (BIA). На **этапе** планирования основное внимание уделяется разработке и реализации стратегий устойчивости и восстановления и их документации в официальных планах непрерывности бизнеса. Наконец, **проверка возможностей проверяет** планы непрерывности бизнеса и их реализаций для проверки эффективности и выявления потенциальных улучшений.

Стратегии непрерывности бизнес-служб Microsoft online используют избыточность оборудования, сети и центра обработки данных. Репликация данных между центрами обработки данных обеспечивает высокую доступность и надежность во время катастрофического инцидента. Это также повышает устойчивость к обыденным инцидентам, таким как изолированные сбои оборудования или повреждения данных.

## <a name="how-does-microsoft-test-business-continuity-and-disaster-recovery-plans"></a>Как Корпорация Майкрософт тестировать непрерывность бизнеса и планы аварийного восстановления?

Политика управления непрерывности Enterprise бизнеса Корпорации Майкрософт предусматривает, что все планы непрерывности бизнеса и аварийного восстановления корпорации Майкрософт должны быть проверены, обновляться и пересматриваться на ежегодной основе. Онлайн-службы Майкрософт тестировать свои планы непрерывности бизнеса по крайней мере ежегодно для политик EBCM. После создания и проверки отчетов Action для проверки результатов тестирования и информирования об обновлениях плана в ответ на любые проблемы, обнаруженные во время тестирования.

Для проверки стратегий устойчивости и восстановления относительно широкого диапазона потенциальных инцидентов программа EBCM определяет несколько категорий тестовых сценариев, влияющих на людей, расположения и технологии. Уровень проверки, требуемый для каждой службы, зависит от ее важности. При этом более важные службы подвергаются более строгой проверке. Каждая команда онлайн-служб Майкрософт проверяет план непрерывности бизнеса в соответствии с рекомендациями EBCM для измерения эффективности плана и готовности группы служб к выполнению плана.

В рамках рекомендаций EBCM ежегодные обзоры планов непрерывности бизнеса и проверки возможностей должны проходить в течение 12 месяцев после последнего обзора. Проверка возможностей должна включать проверку вспомогательной документации, например BIA, чтобы убедиться, что она остается точной. Корпорация Майкрософт делает результаты проверки возможностей для выбора онлайн-служб Майкрософт доступными для наших клиентов с помощью ежеквартных отчетов.

## <a name="how-do-microsoft-online-services-ensure-system-capacity-meets-demand"></a>Каким образом сетевые службы Майкрософт обеспечивают производительность системы, удовлетворяемую спросом?

Планирование емкости помогает группам служб выделять ресурсы, необходимые для поддержки доступности онлайн-служб Майкрософт. Регулярное планирование мощности требуется в рамках программы EBCM корпорации Майкрософт. Группы служб проверяют данные о емкости во время ежеквартных обзоров и во время чрезвычайных ситуаций, которые требуют большей проверки емкости.

Необработанные данные для планирования емкости поддерживаются каждой командой служб и включают такие показатели, как обработка системы, память и аппаратная емкость. Запланированные проверки используют модель текущей емкости системы и тестируют ее относительно прогнозируемых потребностей в экстренных ситуациях. Если модель указывает на недостаток мощности, предложенные изменения мощности системы отправляются руководству команды обслуживания для проверки. Утвержденные изменения включаются в новую модель перед реализацией инженерами команды обслуживания.

## <a name="how-do-microsoft-online-services-maintain-service-availability-during-routine-system-failures"></a>Как сетевые службы Майкрософт поддерживают доступность служб во время обычных сбоев системы?

Веб-службы Майкрософт достигают устойчивости служб за счет избыточной архитектуры, репликации данных и автоматической проверки целостности. Резервная архитектура включает развертывание нескольких экземпляров службы на географическом и физически отдельном оборудовании, обеспечивая повышенную устойчивость к ошибкам для сетевых служб Майкрософт. Репликация данных гарантирует, что в разных зонах сбоя всегда имеется несколько копий данных клиентов, что позволяет восстановить критически важные данные клиента, если они повреждены, потеряны или даже случайно удалены клиентом. Автоматическая проверка целостности повышает доступность данных путем автоматического восстановления данных, на которые влияет множество видов физического или логического повреждения.

## <a name="related-external-regulations--certifications"></a>Связанные внешние правила & сертификации

Онлайн-службы Корпорации Майкрософт регулярно проверяются на соответствие внешним требованиям и сертификациям. Обратитесь к следующей таблице для проверки элементов управления, связанных с устойчивостью и непрерывностью.

### <a name="azure-and-dynamics-365"></a>Azure и Dynamics 365

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.17.1: непрерывность информационной безопасности <br> A.17.2. Избыточность | 2 декабря 2020 г. |
| [ISO 22301](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=6d388547-fc88-46e3-8de2-6bc2edc08b06&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=ee4b611b-bb4d-4056-b189-00da36e88949&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | Все элементы управления | 13 мая 2020 г. |
| [SOC 1;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | BC-1: планы непрерывности бизнеса <br> BC-3: процедуры непрерывности бизнеса и аварийного восстановления <br> BC-4: тестирование BCDR <br> BC-7: планы непрерывности бизнеса центра обработки данных <br> BC-8: тестирование непрерывности бизнеса центра обработки данных <br> BC-9: оценка устойчивости центра обработки данных <br> DS-5: компоненты службы клавиш резервного копирования <br> DS-6: избыточность критически важных компонентов <br> DS-7: автоматическая репликация данных клиентов <br> DS-8: расписание резервного копирования <br> DS-9: процедуры восстановления резервного копирования <br> DS-11: резервные копии offsite <br> DS-14: автоматическое восстановление обслуживания клиентов | 31 марта 2021 г. |

### <a name="office-365"></a>Office 365

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | CP-2. План действий на случай непредвиденных обстоятельств <br> CP-3. Подготовка к непредвиденным ситуациям <br> CP-4: тестирование плана на случай непредвиденных обстоятельств <br> CP-6: альтернативный сайт хранения <br> CP-7: сайт альтернативной обработки <br> CP-9: резервное копирование информационной системы <br> CP-10: восстановление и восстановление информационной системы | 24 сентября 2020 г. |
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.17.1: непрерывность информационной безопасности <br> A.17.2. Избыточность | 20 апреля 2021 г. |
| [ISO 22301](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=13951eb3-6339-4629-b80d-dd0d43812fe7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | Все элементы управления | 18 марта 2019 г. |
| [SOC 1;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-49: политики резервного копирования <br> CA-50: непрерывность бизнеса <br> CA-51: репликация данных | 24 декабря 2020 г. |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-09: восстановление электронной почты EXO | 24 декабря 2020 г. |

## <a name="resources"></a>Ресурсы

- [Whitepaper Enterprise microsoft Enterprise программы управления непрерывности бизнеса](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=64f922a6-d624-40dd-a8ae-6f996b5186f3&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f)
- [Отчет о проверке плана аварийного восстановления Microsoft Cloud EBCM и аварийного восстановления: FY21 Q4](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=83dc940a-2078-4e14-8b7d-07128e5b453d&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_FAQ_and_White_Papers)

## <a name="legal-disclaimer"></a>Юридический отказ

- [Непрерывность бизнес-процессов в компании. Заявление от отказе от ответственности](assurance-ebcm-legal-disclaimer.md)