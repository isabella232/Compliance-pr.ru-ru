---
title: Обзор ведения журнала аудита
description: Сведения о ведении журнала аудита в Microsoft 365
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
ms.openlocfilehash: 3714a5df73253d0814e1d4067248116cb6e10a40
ms.sourcegitcommit: 626b0076d133e588cd28598c149a7f272fc18bae
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2020
ms.locfileid: "49508626"
---
# <a name="audit-logging-overview"></a>Обзор ведения журнала аудита

## <a name="how-does-microsoft-365-employ-audit-logging"></a>Как Microsoft 365 использует ведение журнала аудита?

Microsoft 365 использует ведение журнала аудита для обнаружения неавторизованных действий в своих продуктах и службах и предоставления отчетности для сотрудников Майкрософт. В журналах аудита записываются сведения об изменениях конфигурации системы и событиях доступа, сведения о том, кто отвечает за действие, время и место выполнения действия, а также результат действия. Автоматический анализ журнала поддерживает обнаружение подозрительных поведений в режиме реального времени. Потенциальные происшествия передаются в группу реагирования Microsoft 365 на безопасность для дальнейшего изучения.

Внутреннее ведение журнала аудита Microsoft 365 ведет к сбору данных журнала из различных источников, таких как:

- Журналы событий
- Журналы AppLocker
- Данные о производительности
- System Center Data
- Записи сведений о вызовах
- Данные качества взаимодействия
- Журналы веб-сервера IIS
- Журналы SQL Server
- Данные syslog
- Журналы аудита безопасности

## <a name="how-does-microsoft-365-centralize-and-report-on-audit-logs"></a>Как Microsoft 365 централизовать и отчет о журналах аудита?

Многие типы данных журналов передаются с серверов Microsoft 365 во внутреннюю, общую службу информационных данных с именем Cosmos. Каждая группа обслуживания отправляет журналы аудита из соответствующих серверов в базу данных Cosmos для объединения и анализа. Эта передача данных выполняется через FIPS 140-2-проверенное TLS-подключение на утвержденных портах и протоколах с помощью специализированного средства автоматизации, называемого загрузчиком данных Office (ODL).

Службы Teams запускают запросы в пределах своих данных в Cosmos для корреляции журналов, предупреждений и отчетов. Например, группа безопасности Microsoft 365 использует данные из Cosmos с особым средством синтаксического анализа журнала событий для корреляции данных журнала, отправки оповещений и создания интерактивных отчетов о возможных подозрительных действиях в рабочей среде Microsoft 365. Отчеты из этих данных используются для исправления уязвимостей и повышения общей производительности службы.

## <a name="how-does-microsoft-365-protect-audit-logs"></a>Как Microsoft 365 защищает журналы аудита?

Средства, используемые в Microsoft 365 для сбора и обработки записей аудита, не допускают постоянных или необратимых изменений исходного контента записи аудита или порядка времени. Доступ к данным Microsoft 365, хранящимся в Cosmos, ограничен уполномоченными сотрудниками. Microsoft 365 ограничивает управление функциональными возможностями аудита только ограниченным подмножеством участников группы обслуживания, ответственных за функции аудита. Эти участники группы не могут изменять или удалять данные из Cosmos, а все изменения механизмов ведения журнала для Cosmos записываются и подлежат аудиту. Журналы аудита хранятся достаточно долго для поддержки исследований инцидентов и соблюдения нормативных требований. Точный период хранения данных журнала аудита в Cosmos определяется командами службы. Большинство данных журнала аудита хранятся в течение 90 или более дней.

## <a name="how-does-microsoft-365-protect-end-user-identifiable-information-that-may-be-captured-in-audit-logs"></a>Как Microsoft 365 защищает сведения, идентифицируемые конечными пользователями, которые могут быть захвачены в журналах аудита?

Перед отправкой данных в Cosmos приложение ODL использует службу очистки для маскировки любых полей, содержащих данные клиента, таких как сведения о клиентах и конечных пользователей, и замените эти поля на хэш-значение. Анонимные и хэшированные журналы перезаписываются, а затем передаются в Cosmos.

## <a name="related-external-regulations--certifications"></a>Связанные внешние нормативные & сертификации

Веб-службы корпорации Майкрософт регулярно подлежат аудиту для соответствия внешним нормативам и сертификациям. В следующей таблице приведены сведения о проверке элементов управления, связанных с ведением журнала аудита.

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365)](https://compliance.microsoft.com/compliancemanager) | AU — 2: события аудита <br> AU — 3: содержимое записей аудита <br> AU – 4: аудит емкости хранилища <br> AU – 5: отклик на ошибки при обработке аудита <br> AU — 6: аудит, анализ и создание отчетов <br> AU — 7: сокращение и создание отчетов для аудита <br> AU – 8: отметки времени <br> AU – 9: защита данных аудита  <br> AU – 10: неподдельность <br> AU – 11: хранение записей аудита <br> AU – 12: создание аудита  | 24 сентября 2020 г. | 
| [ISO 27001/27002 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Отчет о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A. 12.4: ведение журнала и мониторинг | 22 февраля 2020 г. |
| [ISO 27017 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Отчет о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A. 12.4: ведение журнала и мониторинг | 22 февраля 2020 г. |
| [SOC 1 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b07c0f7b-6bd5-4544-8255-7a5f14bf914a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Reports) | CA — 48: ведение журнала центра обработки данных <br> CA — 60: ведение журнала аудита | 30 сентября 2019 г. |
| [SOC 2 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=fa062990-e758-4ddc-ace3-7fb21a301d09&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Rep-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Reports) | CA — 48: ведение журнала центра обработки данных <br> CA — 60: ведение журнала аудита | 30 сентября 2019 г. |