---
title: Обзор шифрования и управления ключами
description: Узнайте о шифровании и управлении ключами в Microsoft 365
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
ms.openlocfilehash: dc53f42c6aa7ce16e1291538bfad6d63c5a1689d
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/23/2021
ms.locfileid: "58482011"
---
# <a name="encryption-and-key-management-overview"></a>Обзор шифрования и управления ключами

## <a name="what-role-does-encryption-play-in-protecting-customer-content"></a>Какую роль играет шифрование в защите контента клиента?

Большинство облачных служб Майкрософт являются несколькими клиентами, что означает, что содержимое клиента может храниться на том же физическом оборудовании, что и другие клиенты. Чтобы защитить конфиденциальность контента клиента, онлайн-службы Майкрософт шифруют все данные в покое и в пути с помощью одних из самых надежных и безопасных доступных протоколов шифрования.

Шифрование не заменяет сильное управление доступом. Политика управления доступом Корпорации Майкрософт по нулевому постоянному доступу (ZSA) защищает содержимое клиента от несанкционированного доступа сотрудников Корпорации Майкрософт. Шифрование дополняет управление доступом, защищая конфиденциальность контента клиента, где бы он ни хранился, и не мешая считывке контента во время транзита между системами онлайн-служб Майкрософт или между службами Microsoft Online и клиентом.

## <a name="how-do-microsoft-online-services-encrypt-data-at-rest"></a>Как сетевые службы Майкрософт шифруют данные на отдыхе?

Все содержимое клиента в сетевых службах Майкрософт защищено одной или несколько форм шифрования. Серверы Майкрософт используют BitLocker для шифрования дисков, содержащих содержимое клиента на уровне громкости. Шифрование, предоставляемого BitLocker, защищает содержимое клиента, если существуют упущения в других процессах или средствах управления (например, управление доступом или рециркуляция оборудования), которые могут привести к несанкционированному физическому доступу к дискам, содержащим содержимое клиента.

Помимо шифрования на уровне громкости, веб-службы Майкрософт используют шифрование служб на уровне приложений для шифрования контента клиентов. Шифрование служб обеспечивает защиту прав и функции управления на вершине сильной защиты шифрования. Он также позволяет отделять Windows операционные системы от данных клиентов, хранимых или обрабатываемых этими операционными системами.

## <a name="how-do-microsoft-online-services-encrypt-data-in-transit"></a>Как интернет-службы Майкрософт шифруют данные при транзите?

Сетевые службы Майкрософт используют сильные транспортные протоколы, такие как TLS, чтобы предотвратить прослушивание неавторизованной стороной данных клиентов во время перемещения по сети. Примеры транзитных данных включают почтовые сообщения, которые находятся в процессе доставки, беседы, происходящие в онлайн-собрании, или файлы, реплицированные между центрами обработки данных.

Для сетевых служб Майкрософт данные считаются "транзитными" при общении устройства пользователя с сервером Майкрософт или сервера Майкрософт с другим сервером.

## <a name="how-do-microsoft-online-services-manage-the-keys-used-for-encryption"></a>Как сетевые службы Майкрософт управляют ключами, используемыми для шифрования?

Надежное шифрование является безопасным только для ключей, используемых для шифрования данных. Корпорация Майкрософт использует собственные сертификаты безопасности для шифрования подключений TLS для передачи данных. Для данных на отдыхе объемы, защищенные BitLocker, шифруются с ключом шифрования полного объема, который шифруется ключом магистрали тома, который, в свою очередь, связан с доверенным модулем платформы (TPM) на сервере. BitLocker использует алгоритмы, совместимые с FIPS, чтобы гарантировать, что ключи шифрования никогда не хранятся и не отправляются по проводу в чистом.

Шифрование службы обеспечивает еще один уровень шифрования для клиентской базы данных на отдыхе, предоставляя клиентам два варианта управления ключами шифрования: клавиши с управлением Майкрософт или ключ клиента. При использовании ключей, управляемых Корпорацией Майкрософт, сетевые службы Майкрософт автоматически создают и надежно хранят корневые ключи, используемые для шифрования служб.

Клиенты с требованиями для управления собственными ключами корневого шифрования могут использовать шифрование службы с ключом клиента. С помощью ключа клиента клиенты могут создавать собственные криптографические ключи с помощью локального модуля службы оборудования (HSM) или хранилища ключей Azure (AKV). Корневые ключи клиента хранятся в AKV, где они могут использоваться в качестве корневого ключа одного из ключей, шифруемого данными или файлами почтовых ящиков клиентов. Корневые ключи клиента могут быть доступны только косвенно кодом онлайн-службы Майкрософт для шифрования данных и не могут быть доступны непосредственно сотрудниками Корпорации Майкрософт.

## <a name="related-external-regulations--certifications"></a>Связанные внешние правила & сертификации

Онлайн-службы Корпорации Майкрософт регулярно проверяются на соответствие внешним требованиям и сертификациям. Обратитесь к следующей таблице для проверки элементов управления, связанных с шифрованием и управлением ключами.

### <a name="azure-and-dynamics-365"></a>Azure и Dynamics 365

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.10.1: элементы управления криптографией <br> A.18.1.5: элементы управления криптографией | 2 декабря 2020 г. |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.10.1: элементы управления криптографией <br> A.18.1.5: элементы управления криптографией | 2 декабря 2020 г. |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=56904fc3-0942-4ff5-9eef-7cabc751a25c&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.11.6. Шифрование PII, передаваемого через общедоступные сети передачи данных | 2 декабря 2020 г. |
| [SOC 1;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | DS-1: безопасное хранение криптографических сертификатов и ключей <br> DS-2: данные клиента шифруются при транзите <br> DS-3: внутренняя связь компонентов Azure, зашифрованных во время транзита <br> DS-4: криптографические элементы управления и процедуры | 31 марта 2021 г. |

### <a name="office-365"></a>Office 365

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | SC-8: конфиденциальность и целостность передачи <br> SC-13: использование криптографии <br> SC-28: защита информации в покое <br>  | 24 сентября 2020 г. |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.10.1: элементы управления криптографией <br> A.18.1.5: элементы управления криптографией | 20 апреля 2021 г. |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.11.6. Шифрование PII, передаваемого через общедоступные сети передачи данных | 20 апреля 2021 г. |
| [SOC 2;](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-44: шифрование данных в транзите <br> CA-54: шифрование данных на отдыхе <br> CA-62: шифрование почтовых ящиков ключа клиента <br> CA-63: удаление данных ключа клиента <br> CA-64: ключ клиента | 24 декабря 2020 г. |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-16: ключи шифрования клиентов <br> CUEC-17: хранилище ключей клиента <br>  CUEC-18: ротация ключей клиента| 24 декабря 2020 г. |
