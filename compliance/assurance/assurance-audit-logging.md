---
title: Обзор журнала аудита
description: Узнайте о logging аудита в Microsoft 365
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
ms.openlocfilehash: 6e32e089a5b42f846a332e32218959fef5103615
ms.sourcegitcommit: 7a5b6bc58fc4613b38f3fda20aebee5cec6a5730
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49787508"
---
# <a name="audit-logging-overview"></a>Обзор журнала аудита

## <a name="how-does-microsoft-365-employ-audit-logging"></a>Как Microsoft 365 использует ведение журнала аудита?

Microsoft 365 использует ведение журнала аудита для обнаружения несанкционированных действий в своих продуктах и службах и обеспечения ответственности за персонал Корпорации Майкрософт. В журналах аудита регистрются сведения об изменениях конфигурации системы и событиях доступа, с подробными сведениями, чтобы определить, кто несет ответственность за действие, когда и где произошло действие, а также результат действия. Автоматический анализ журналов поддерживает обнаружение подозрительного поведения почти в реальном времени. Для дальнейшего расследования потенциальные инциденты передается в службу реагирования на угрозы безопасности Microsoft 365.

Ведение журнала внутреннего аудита Microsoft 365 захватывает данные журнала из различных источников, например:

- Журналы событий
- Журналы AppLocker
- Данные о производительности
- Данные System Center
- Записи подробных вызовов
- Данные о качестве работы
- Журналы веб-сервера IIS
- SQL Server журналов
- Данные Syslog
- Журналы аудита безопасности

## <a name="how-does-microsoft-365-centralize-and-report-on-audit-logs"></a>Как Microsoft 365 централизует журналы аудита и сообщает о них?

Многие типы данных журнала загружаются с серверов Microsoft 365 во внутреннюю вычислительную службу больших данных Cosmos. Каждая группа служб загружает журналы аудита с соответствующих серверов в базу данных Cosmos для агрегации и анализа. Эта передача данных происходит через подключение TLS с проверкой FIPS 140-2 на утвержденных портах и протоколах с помощью проприетарного средства автоматизации, называемого загрузчиком данных Office (ODL).

Группы обслуживания запускают запросы на основе областей к своим данным в Cosmos для корреляции журнала, оповещения и отчетности. Например, группа безопасности Microsoft 365 использует данные из Cosmos с проприетарным анализером журнала событий для корреляции данных журнала, отправки оповещений и создания отчетов о возможных подозрительных действиях в производственной среде Microsoft 365. Отчеты из этих данных используются для устранения уязвимостей и повышения общей производительности службы.

## <a name="how-does-microsoft-365-protect-audit-logs"></a>Как Microsoft 365 защищает журналы аудита?

Средства, используемые в Microsoft 365 для сбора и обработки записей аудита, не позволяют вносить постоянные или необратимые изменения в исходное содержимое записей аудита или порядок времени. Доступ к данным Microsoft 365, хранимых в Cosmos, разрешен только полномочным сотрудникам. Microsoft 365 ограничивает управление функциями аудита ограниченной частью участников группы обслуживания, которые отвечают за функции аудита. Эти участники группы не могут изменять или удалять данные из Cosmos, а все изменения механизмов ведения журнала для Cosmos записываюются и проверяются. Журналы аудита сохраняются достаточно долго, чтобы поддерживать расследования инцидентов и соответствовать нормативным требованиям. Точный период хранения данных журнала аудита в Cosmos определяется группами служб; большинство данных журнала аудита сохраняется в течение 90 дней или более.

## <a name="how-does-microsoft-365-protect-end-user-identifiable-information-that-may-be-captured-in-audit-logs"></a>Как Microsoft 365 защищает зависимые от пользователя сведения, которые могут быть захвачены в журналах аудита?

Перед отправкой данных в Cosmos приложение ODL использует службу очистки, чтобы обфускировать любые поля, содержащие данные клиента, например сведения о клиенте и информацию, идентифицируемую конечным пользователем, и заменить эти поля на значение hash. Анонимизированные и hashed журналы переописываются, а затем загружаются в Cosmos.

## <a name="related-external-regulations--certifications"></a>Связанные внешние нормативы & сертификации

Веб-службы Майкрософт регулярно проверяются на соответствие внешним нормативным требованиям и сертификациям. Проверка элементов управления, связанных с ведением журнала аудита, приводится в следующей таблице.

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365)](https://compliance.microsoft.com/compliancemanager) | AU-2: события аудита <br> AU-3: содержимое записей аудита <br> AU-4: аудит емкости хранилища <br> AU-5: реагирование на сбои обработки аудита <br> AU-6: аудит проверки, анализа и отчетности <br> AU-7: сокращение аудита и генерация отчетов <br> AU-8: отметки времени <br> AU-9: защита информации аудита  <br> AU-10: неопубликовка <br> AU-11: хранение записей аудита <br> AU-12: генерация аудита  | 24 сентября 2020 г. | 
| [ISO 27001/27002 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Заявление о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.4: ведение журнала и мониторинг | 22 февраля 2020 г. |
| [ISO 27017 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Заявление о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.4: ведение журнала и мониторинг | 22 февраля 2020 г. |
| [SOC 1 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-48: ведение журнала центра обработки данных <br> CA-60: ведение журнала аудита | 24 декабря 2020 г. |
| [SOC 2 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-48: ведение журнала центра обработки данных <br> CA-60: ведение журнала аудита | 24 декабря 2020 г.|