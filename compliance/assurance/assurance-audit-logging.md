---
title: Обзор журнала аудита
description: Узнайте о журнале аудита в Microsoft 365
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
ms.openlocfilehash: dc56d0413811d59309c974931e1fa50ee184e94a
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51497682"
---
# <a name="audit-logging-overview"></a>Обзор журнала аудита

## <a name="how-does-microsoft-365-employ-audit-logging"></a>Как в Microsoft 365 применяются журналы аудита?

Корпорация Майкрософт 365 использует журнал аудита для обнаружения несанкционированных действий в своих продуктах и службах и обеспечения подотчетности сотрудников Корпорации Майкрософт. Журналы аудита фиксировать сведения об изменениях конфигурации системы и событиях доступа, а также сведения о том, кто несет ответственность за эту деятельность, когда и где она проводилась, и каковы результаты этого действия. Автоматизированный анализ журналов поддерживает обнаружение подозрительного поведения в режиме реального времени. Возможные инциденты переназяются в команду реагирования на безопасность Microsoft 365 для дальнейшего расследования.

Внутренний журнал аудита Microsoft 365 захватывает данные журналов из различных источников, таких как:

- Журналы событий
- Журналы AppLocker
- Данные о производительности
- Данные Центра систем
- Записи детализации вызовов
- Качество данных об опыте
- Журналы веб-сервера IIS
- SQL Server журналы
- Данные Syslog
- Журналы аудита безопасности

## <a name="how-does-microsoft-365-centralize-and-report-on-audit-logs"></a>Как Microsoft 365 централизует журналы аудита и сообщает о них?

Многие типы данных журнала загружаются с серверов Microsoft 365 во внутреннюю службу вычислений больших данных под названием Cosmos. Каждая группа служб загружает журналы аудита с соответствующих серверов в базу данных Cosmos для агрегации и анализа. Этот перенос данных происходит через подключение TLS с проверкой FIPS 140-2 в утвержденных портах и протоколах с помощью средства автоматизации Office Data Loader (ODL).

Группы служб запускают объемные запросы по своим данным в Космосе для корреляции журналов, оповещения и отчетов. Например, группа безопасности Microsoft 365 использует данные из Cosmos с несвободным анализом журналов событий для сопоставления данных журналов, отправки оповещений и создания отчетов о возможной подозрительной активности в среде производства Microsoft 365. Отчеты из этих данных используются для устранения уязвимостей и повышения общей производительности службы.

## <a name="how-does-microsoft-365-protect-audit-logs"></a>Как Microsoft 365 защищает журналы аудита?

Средства, используемые в Microsoft 365 для сбора и обработки записей аудита, не позволяют вносить постоянные или необратимые изменения в исходное содержимое записи аудита или порядок времени. Доступ к данным Microsoft 365, хранимым в Космосе, ограничен уполномоченным персоналом. Microsoft 365 ограничивает управление функциями аудита ограниченным подмножеством членов группы служб, отвечающих за функции аудита. Эти члены группы не имеют возможности изменять или удалять данные из Cosmos, и все изменения в механизмах ведения журнала для Cosmos записывают и проверяют. Журналы аудита сохраняются достаточно долго, чтобы поддерживать расследования инцидентов и соответствовать нормативным требованиям. Точный период хранения данных журнала аудита в Космосе определяется группами служб; большинство данных журнала аудита сохраняется в течение 90 дней или дольше.

## <a name="how-does-microsoft-365-protect-end-user-identifiable-information-that-may-be-captured-in-audit-logs"></a>Как Microsoft 365 защищает идентифицируемые данные конечных пользователей, которые могут быть запечатлены в журналах аудита?

Перед отправкой данных в Cosmos приложение ODL использует службу очистки, чтобы заместить все поля, содержащие данные клиентов, такие как данные клиента и идентифицируемую конечным пользователем информацию, и заменить эти поля значением hash. Анонимизированные и хашизированные журналы переписываются и затем загружаются в Cosmos.

## <a name="related-external-regulations--certifications"></a>Связанные внешние правила & сертификации

Онлайн-службы Корпорации Майкрософт регулярно проверяются на соответствие внешним требованиям и сертификациям. Обратитесь к следующей таблице для проверки элементов управления, связанных с ведением журнала аудита.

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365)](https://compliance.microsoft.com/compliancemanager) | AU-2: события аудита <br> AU-3: содержимое записей аудита <br> AU-4: емкость хранилища аудита <br> AU-5: реагирование на сбои в обработке аудита <br> AU-6: аудит, анализ и отчетность <br> AU-7: сокращение аудита и генерация отчетов <br> AU-8: штампы времени <br> AU-9. Защита сведений о аудите  <br> AU-10: неопубликовка <br> AU-11: хранение записей аудита <br> AU-12: генерация аудита  | 24 сентября 2020 г. | 
| [ISO 27001/27002 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.4. Ведение журнала и мониторинг | 22 февраля 2020 г. |
| [ISO 27017 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.4. Ведение журнала и мониторинг | 22 февраля 2020 г. |
| [SOC 1 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-48. Журнал центра обработки данных <br> CA-60: журнал аудита | 24 декабря 2020 г. |
| [SOC 2 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-48. Журнал центра обработки данных <br> CA-60: журнал аудита | 24 декабря 2020 г.|