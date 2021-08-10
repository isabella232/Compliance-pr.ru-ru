---
title: Обзор управления поставщиками
description: Узнайте об управлении поставщиками в Microsoft 365
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: article
f1.keywords:
- NOCSH'
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
ms.openlocfilehash: abf8616033ee8046447b0d10292ddd25278a29a31ad829c9e0a97df7d11e2271
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54291737"
---
# <a name="supplier-management-overview"></a>Обзор управления поставщиками

## <a name="how-does-microsoft-manage-risk-related-to-suppliers"></a>Как Корпорация Майкрософт управляет рисками, связанными с поставщиками?

Корпорация Майкрософт партнеров с сторонними компаниями, чтобы помочь удовлетворить потребности наших клиентов. Эти сторонние компании называются поставщиками или субпроцессорами. Безопасность и конфиденциальность поставщиков в Корпорации Майкрософт регулируются нашей программой обеспечения безопасности и конфиденциальности поставщиков [(SSPA)](https://www.microsoft.com/procurement/sspa?activetab=pivot1%3aprimaryr6)— корпоративным набором требований для всех поставщиков, сотрудничающих с Корпорацией Майкрософт, для предоставления наших онлайн-служб. Хотя программа SSPA обеспечивает комплексное управление и управление базой поставщиков, отдельные бизнес-подразделения могут поддерживать дополнительные требования к своим поставщикам.

## <a name="how-does-microsofts-supplier-security-and-privacy-assurance-sspa-program-protect-customer-data"></a>Как программа обеспечения безопасности и конфиденциальности поставщиков Майкрософт (SSPA) защищает данные клиентов?

SSPA — это партнерство между корпорацией Майкрософт по закупкам, корпоративным внешним и юридическим вопросам и корпоративной безопасности, чтобы обеспечить соблюдение поставщиками принципов конфиденциальности и безопасности Корпорации Майкрософт. Область SSPA охватывает всех поставщиков, которые обрабатывает персональные данные или конфиденциальные данные Майкрософт. Регистрация программы SSPA включает соблюдение требований Майкрософт по защите данных (DPR). DPR состоит из элементов управления безопасностью и конфиденциальностью, которые поставщики должны реализовать перед началом контрактной работы с Корпорацией Майкрософт. Все зарегистрированные поставщики самостоятельно подтверждают соответствие требованиям ДНР ежегодно.

Требования DPR в области основаны на шести отдельных категориях обработки данных, для которые поставщик может быть утвержден в рамках их регистрации в SSPA. Эти категории используются для определения риска, связанного с службами, которые поставщик предоставляет Корпорации Майкрософт. Профиль обработки данных поставщика определяет, какие элементы управления DPR считаются в области обеспечения соответствующей защиты данных. Поставщики, которые обрабатывает данные, которые считаются более высокими рисками, должны соответствовать всем требованиям ДНР, а также должны обеспечить независимую проверку соответствия требованиям. Средства покупки Майкрософт проверяют состояние SSPA всех поставщиков, включая соответствие применимым частям ДНР, прежде чем разрешить закупку этого поставщика.

## <a name="what-types-of-subprocessors-provide-services-for-microsoft"></a>Какие типы субпроцессоров предоставляют службы для Корпорации Майкрософт?

Подпроцессор — это третья сторона, в обязанности которой входит обработка персональных данных Майкрософт, для которой Корпорация Майкрософт является процессором. Подпроцессоры Майкрософт подпадают под три различные категории. Каждый должен продемонстрировать соответствие требованиям SSPA, прежде чем обрабатывать данные о клиентах от имени Корпорации Майкрософт.

- Дополнительные обработчики данных **технологий** предоставляют технологии, используемые для предоставления определенных веб-служб Майкрософт. Если клиент развертывает одну из этих служб, подпроцессоры, указанные для этой службы, могут обрабатывать, хранить или иным образом получать доступ к данным клиентов или личным данным, помогая предоставлять эту службу.
- **Дополнительные** подпроцессоры предоставляют службы, которые поддерживают, работают и поддерживают онлайн-службы. Если клиент развертывает одну из этих служб, указанные подпроцессоры могут обрабатывать, хранить или иным образом получать доступ к ограниченным данным клиента или личным данным при предоставлении дополнительных служб.
- **Подпроцессоры** по увеличению персонала принимают две различные формы: в обоих сценариях персональные данные находятся только в объектах Майкрософт, в системах Майкрософт и подчиняются политикам и надзору Корпорации Майкрософт.

    - Первая форма расширения персонала обеспечивает персонал, который поддерживает, управляет и поддерживает веб-службы Майкрософт. При выполнении своих обязанностей эти дополнительные обработчики данных могут иметь доступ к данным клиентов или личным данным. Например, дополнительный обработчик данных может выполнять удаленное устранение неполадок на сервере Майкрософт и при этом может получать доступ к фрагментам данных клиента в журнале аварийного дампа сервера.
    - Вторая форма увеличения штата включает в себя субпроцессоры, которые работают бок о бок с сотрудниками Корпорации Майкрософт, работающими полный рабочий день, для поддержки, работы и обслуживания сетевых служб Майкрософт. Эти дополнительные обработчики служб могут получать доступ к псевдонимизированным данным в рамках своей работы вместе с штатными сотрудниками Майкрософт.

Для реализации элементов управления доступом в соответствии с требованиями Майкрософт по защите данных (DPR) необходимы технологии и дополнительные подпроцессоры. Эти требования соответствуют или превышают обязательства корпорации Майкрософт по контрактам перед клиентами в условиях обслуживания в Интернете (OST). Поставщики, которые выполняют работу по увеличению персонала, должны иметь те же элементы управления доступом, что и сотрудники Корпорации Майкрософт, работающие полный рабочий день.

## <a name="how-does-microsoft-onboard-suppliers"></a>Как microsoft onboard suppliers?

Сторонние поставщики должны подписывать мастер-соглашение Microsoft в рамках процесса работы с бортовой записью. Это соглашение регулирует отношения между Корпорацией Майкрософт и ее поставщиками и обеспечивает последовательное управление отношениями поставщиков. В рамках onboarding поставщики зарегистрировались в SSPA и должны выполнить все применимые требования, прежде чем они могут быть утверждены для любых категорий обработки данных. Бизнес-подразделения Майкрософт могут создавать взаимодействия с поставщиками только в том случае, если процесс обработки данных для участия соответствует категориям обработки данных, для которых был утвержден поставщик.

## <a name="how-does-microsoft-notify-customers-of-changes-to-suppliers-who-process-their-data"></a>Как Корпорация Майкрософт уведомляет клиентов об изменениях поставщиков, которые обрабатывает их данные?

В дополнение к защите данных microsoft Online Service Data Protection (DPA) Корпорация Майкрософт принимает дополнительные обязательства в отношении периодов уведомления о добавлении любого подпроцессора. Сроки уведомления зависят от типа данных, которые будет обрабатывать подпроцессор от имени Корпорации Майкрософт. Как указано в DPA, Корпорация Майкрософт обязуется предоставлять уведомления клиентам не менее чем за шесть месяцев до любого нового подпроцессора, который будет обрабатывать данные клиента. Для любых других персональных данных Корпорация Майкрософт предоставит уведомление не менее чем за 30 дней. Уведомление предоставляется обновлением списка [Microsoft Online Services subprocessor.](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=926b2cf5-6b6e-43ca-9bc3-f73e961aad5f&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_Subprocessor_List)

## <a name="related-external-regulations--certifications"></a>Связанные внешние правила & сертификации

Онлайн-службы Корпорации Майкрософт регулярно проверяются на соответствие внешним требованиям и сертификациям. Обратитесь к приведенной ниже таблице для проверки элементов управления, связанных с управлением поставщиками.

### <a name="azure-and-dynamics-365"></a>Azure и Dynamics 365

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|  
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.15.1. Информационная безопасность в отношениях поставщиков | 2 декабря 2020 г. |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.15.1. Информационная безопасность в отношениях поставщиков | 2 декабря 2020 г. |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=56904fc3-0942-4ff5-9eef-7cabc751a25c&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) |  A.8.1. Раскрытие субподрядной обработки PII | 2 декабря 2020 г. |
| [SOC 2;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | SOC2-25: управление рисками поставщика <br> C5-2: обзор профилей рисков поставщика| 31 марта 2021 г. |

### <a name="office-365"></a>Office 365

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|  
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | CA-3: системные взаимосвязи <br> IA-4: управление идентификаторами <br> PS-6. Соглашения о доступе <br> PS-7: безопасность сторонних сотрудников <br> SA-4: процесс приобретения <br> SA-9: внешние службы информационной системы <br> SA-12: защита цепочки поставок | 24 сентября 2020 г. |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.15.1. Информационная безопасность в отношениях поставщиков | 20 апреля 2021 г. |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) |  A.8.1. Раскрытие субподрядной обработки PII | 24 декабря 2020 г. |
| [SOC 2;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-53: сторонний мониторинг | 24 декабря 2020 г. |

## <a name="resources"></a>Ресурсы

- [Программа обеспечения конфиденциальности и обеспечения безопасности поставщиков](https://www.microsoft.com/procurement/sspa?activetab=pivot1%3aprimaryr6)
