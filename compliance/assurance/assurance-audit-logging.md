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
ms.openlocfilehash: e6bf564f182f2dfabc6561602e5a4cb5c8c3445e
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53088691"
---
# <a name="audit-logging-overview"></a>Обзор журнала аудита

## <a name="how-does-microsoft-365-employ-audit-logging"></a>Как Microsoft 365 использовать журнал аудита?

Microsoft 365 для обнаружения несанкционированных действий в своих продуктах и службах и обеспечения подотчетности сотрудников Корпорации Майкрософт. Журналы аудита фиксировать сведения об изменениях конфигурации системы и событиях доступа, а также сведения о том, кто несет ответственность за эту деятельность, когда и где она проводилась, и каковы результаты этого действия. Автоматизированный анализ журналов поддерживает обнаружение подозрительного поведения в режиме реального времени. Возможные инциденты переназяются в Microsoft 365 безопасности для дальнейшего расследования.

Microsoft 365 ведения журнала аудита захватывает данные журналов из различных источников, таких как:

- Журналы событий
- Журналы AppLocker
- Данные о производительности
- System Center данных
- Записи детализации вызовов
- Качество данных об опыте
- Журналы веб-сервера IIS
- SQL Server журналы
- Данные Syslog
- Журналы аудита безопасности

## <a name="how-does-microsoft-365-centralize-and-report-on-audit-logs"></a>Как Microsoft 365 централизовать журналы аудита и сообщать о них?

Многие типы данных журналов загружаются с Microsoft 365 серверов в несвободное решение мониторинга безопасности для анализа в режиме реального времени (NRT) и внутреннюю службу вычислений больших данных (Cosmos) для долгосрочного хранения. Этот перенос данных происходит через подключение TLS с проверкой FIPS 140-2 в утвержденных портах и протоколах с помощью средства собственной автоматизации, называемого погрузчиком данных Office (ODL).

Журналы обрабатываются в NRT с помощью методов, основанных на правилах, статистических данных и машинного обучения для обнаружения показателей производительности системы и потенциальных событий безопасности. Модели машинного обучения используют входящие данные журнала и исторические данные журнала, хранимые в Cosmos для непрерывного улучшения возможностей обнаружения. Обнаружения, связанные с безопасностью, создают оповещения, оповещают дежурных инженеров о потенциальном инциденте и запускают автоматические действия по исправлению, если это применимо. Кроме автоматического мониторинга безопасности, группы служб используют средства анализа и панели мониторинга для корреляции данных, интерактивных запросов и аналитики данных. Эти отчеты используются для мониторинга и повышения общей производительности службы.

Дополнительные сведения о мониторинге безопасности и оповещении см. в [обзоре мониторинга безопасности.](assurance-security-monitoring.md)

![Поток данных аудита](../media/assurance-audit-data-flow.png)

## <a name="how-does-microsoft-365-protect-audit-logs"></a>Как Microsoft 365 журналы аудита?

Средства, используемые в Microsoft 365 для сбора и обработки записей аудита, не позволяют вносить постоянные или необратимые изменения в исходное содержимое записи аудита или порядок времени. Доступ к Microsoft 365, хранимых в Cosmos, ограничен уполномоченным персоналом. Кроме того, Microsoft 365 ограничивает управление журналами аудита ограниченным подмножеством членов группы безопасности, отвечающих за функции аудита. Группа безопасности не имеет постоянного административного доступа к Cosmos. Для административного доступа требуется утверждение доступа к just-in-time (JIT), и все изменения в механизмах ведения журнала для Cosmos записывают и проверяют. Журналы аудита сохраняются достаточно долго, чтобы поддерживать расследования инцидентов и соответствовать нормативным требованиям. Точный период хранения данных журнала аудита в Cosmos определяется группами служб; большинство данных журнала аудита сохраняется в течение 90 дней или дольше.

## <a name="how-does-microsoft-365-protect-end-user-identifiable-information-that-may-be-captured-in-audit-logs"></a>Как Microsoft 365 защитить идентифицируемые сведения, которые могут быть запечатлены в журналах аудита?

Перед отправкой данных журнала приложение ODL использует службу очистки для удаления полей, содержащих данные клиентов, таких как сведения о клиентах и идентифицируемых данных конечных пользователей, а также для замены этих полей значением hash. Анонимизированные и схващенные журналы переписываются и затем загружаются в Cosmos. Все передачи журналов происходят через зашифрованное подключение TLS (FIPS 140-2).

## <a name="related-external-regulations--certifications"></a>Связанные внешние правила & сертификации

Онлайн-службы Корпорации Майкрософт регулярно проверяются на соответствие внешним требованиям и сертификациям. Обратитесь к следующей таблице для проверки элементов управления, связанных с ведением журнала аудита.

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365)](https://compliance.microsoft.com/compliancemanager) | AU-2: события аудита <br> AU-3: содержимое записей аудита <br> AU-4: емкость хранилища аудита <br> AU-5: реагирование на сбои в обработке аудита <br> AU-6: аудит, анализ и отчетность <br> AU-7: сокращение аудита и генерация отчетов <br> AU-8: штампы времени <br> AU-9. Защита сведений о аудите  <br> AU-10: неопубликовка <br> AU-11: хранение записей аудита <br> AU-12: генерация аудита  | 24 сентября 2020 г. | 
| [ISO 27001/27002 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.4. Ведение журнала и мониторинг | 20 апреля 2021 г. |
| [ISO 27017 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.12.4. Ведение журнала и мониторинг | 20 апреля 2021 г. |
| [SOC 1 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-48. Журнал центра обработки данных <br> CA-60: журнал аудита | 24 декабря 2020 г. |
| [SOC 2 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-48. Журнал центра обработки данных <br> CA-60: журнал аудита | 24 декабря 2020 г.|