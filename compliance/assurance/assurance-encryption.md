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
ms.openlocfilehash: 5e46fdb5ddc3b1b80df0bcadf9054b9353a0dc8e
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53088648"
---
# <a name="encryption-and-key-management-overview"></a>Обзор шифрования и управления ключами

## <a name="what-role-does-encryption-play-in-protecting-customer-content"></a>Какую роль играет шифрование в защите контента клиента?

Большинство облачных служб Майкрософт являются многоуровневые, что означает, что содержимое клиента может храниться на том же физическом оборудовании, что и другие клиенты. Чтобы защитить конфиденциальность контента клиента, Microsoft 365 шифрует все данные в покое и в пути с помощью самых надежных и безопасных доступных протоколов шифрования.

Шифрование не заменяет сильное управление доступом. Microsoft 365 политики управления доступом нулевого постоянного доступа (ZSA) защищает содержимое клиента от несанкционированного доступа сотрудников Майкрософт. Шифрование дополняет управление доступом, защищая конфиденциальность контента клиента везде, где он хранится, и не мешая считываемому контенту во время транзита между Microsoft 365 системами или между Microsoft 365 и клиентом.

## <a name="how-does-microsoft-365-encrypt-data-at-rest"></a>Как Microsoft 365 шифрование данных на отдыхе?

Все содержимое клиента в Microsoft 365 защищено одной или несколько форм шифрования. Серверы Майкрософт используют BitLocker для шифрования дисков, содержащих содержимое клиента на уровне громкости. Шифрование, предоставляемого BitLocker, защищает содержимое клиента в случае неявок в другие процессы или элементы управления (например, управление доступом или повторное использование оборудования), что может привести к несанкционированному физическому доступу к дискам, содержащим содержимое клиента.

Exchange Online, Microsoft Teams, SharePoint Online и OneDrive для бизнеса шифрование служб на уровне приложения для шифрования контента клиентов. Шифрование служб обеспечивает защиту прав и функции управления на вершине сильной защиты шифрования. Он также позволяет отделять Windows операционные системы от данных клиентов, хранимых или обрабатываемых этими операционными системами.

## <a name="how-does-microsoft-365-encrypt-data-in-transit"></a>Как Microsoft 365 шифрование данных при транзите?

Microsoft 365 и службы используют прочные транспортные протоколы, такие как TLS, чтобы предотвратить прослушивание неавторизованной стороной данных клиентов во время перемещения по сети. Примеры транзитных данных включают почтовые сообщения, которые находятся в процессе доставки, беседы, происходящие в онлайн-собрании, или файлы, реплицированные между центрами обработки данных.

В Microsoft 365, данные считаются "в пути" всякий раз, когда устройство пользователя общается с сервером Майкрософт или серверОм Майкрософт, общаясь с другим сервером. Exchange Online, SharePoint Online, Microsoft Teams и Office Online используют TLS для обеспечения конфиденциальности данных во время транзита.

## <a name="how-does-microsoft-365-manage-the-keys-used-for-encryption"></a>Как Microsoft 365 управлять ключами, используемыми для шифрования?

Надежное шифрование является безопасным только для ключей, используемых для шифрования данных. Корпорация Майкрософт использует собственные сертификаты безопасности для шифрования подключений TLS для передачи данных. Для данных на отдыхе объемы, защищенные BitLocker, шифруются с ключом шифрования полного объема, который шифруется ключом магистрали тома, который, в свою очередь, связан с доверенным модулем платформы (TPM) на сервере. BitLocker использует алгоритмы, совместимые с FIPS, чтобы гарантировать, что ключи шифрования никогда не хранятся и не отправляются по проводу в чистом.

Шифрование служб обеспечивает дополнительный уровень шифрования данных клиентов в Exchange Online, Microsoft Teams, SharePoint Online и OneDrive для бизнеса. Шифрование служб предоставляет клиентам два варианта управления ключами шифрования: клавиши с управлением Майкрософт или клиентский ключ. При использовании ключей с управлением Майкрософт Microsoft 365 автоматически генерируют и надежно хранят корневые ключи, используемые для шифрования служб.

Клиенты с требованиями для управления собственными ключами корневого шифрования могут использовать шифрование служб с помощью ключа клиента. С помощью ключа клиента клиенты могут создавать собственные криптографические ключи с помощью локального модуля службы оборудования (HSM) или хранилища ключей Azure (AKV). Корневые ключи клиента хранятся в AKV, где они могут использоваться в качестве корневого ключа одного из ключей, шифруемого данными или файлами почтовых ящиков клиентов. К корневым ключам клиента можно получить Microsoft 365 код службы для шифрования данных, а непосредственно к ним не могут обратиться сотрудники Корпорации Майкрософт.

## <a name="related-external-regulations--certifications"></a>Связанные внешние правила & сертификации

Онлайн-службы Корпорации Майкрософт регулярно проверяются на соответствие внешним требованиям и сертификациям. Обратитесь к следующей таблице для проверки элементов управления, связанных с шифрованием и управлением ключами.

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365)](https://compliance.microsoft.com/compliancemanager) | SC-8: конфиденциальность и целостность передачи <br> SC-13: использование криптографии <br> SC-28: защита информации в покое <br>  | 24 сентября 2020 г. |
| [ISO 27001/27002 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.10.1: элементы управления криптографией <br> A.18.1.5: элементы управления криптографией | 20 апреля 2021 г. |
| [ISO 27017 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.10.1: элементы управления криптографией <br> A.18.1.5: элементы управления криптографией | 20 апреля 2021 г. |
| [ISO 27018 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Утверждение применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=43e89534-f48d-42ea-a7a7-3523ff516036&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.11.6. Шифрование PII, передаваемого через общедоступные сети передачи данных | 20 апреля 2021 г. |
| [SOC 2 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-44: шифрование данных в транзите <br> CA-54: шифрование данных на отдыхе <br> CA-62: шифрование почтовых ящиков ключа клиента <br> CA-63: удаление данных ключа клиента <br> CA-64: ключ клиента | 24 декабря 2020 г. |
| [SOC 3 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-16: ключи шифрования клиентов <br> CUEC-17: хранилище ключей клиента <br>  CUEC-18: ротация ключей клиента| 24 декабря 2020 г. |
