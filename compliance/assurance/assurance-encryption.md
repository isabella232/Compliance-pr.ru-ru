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
ms.openlocfilehash: ca13c5dfb229acd46ef0dd027b537afc2ac20b5a
ms.sourcegitcommit: 7a5b6bc58fc4613b38f3fda20aebee5cec6a5730
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49787348"
---
# <a name="encryption-and-key-management-overview"></a>Обзор шифрования и управления ключами

## <a name="what-role-does-encryption-play-in-protecting-customer-content"></a>Какую роль играет шифрование в защите контента клиента?

Большинство облачных служб Майкрософт для бизнеса являются мультитенантными, то есть контент клиентов может храниться на том же физическом оборудовании, что и другие клиенты. Чтобы защитить конфиденциальность контента клиента, Microsoft 365 шифрует все неавтомтные данные и передает их с помощью самых надежных и безопасных протоколов шифрования.

Шифрование не заменяет собой мощные элементы управления доступом. Политика контроля доступа Microsoft 365 в отношении нулевого постоянного доступа (ZSA) защищает содержимое клиентов от несанкционированного доступа сотрудников Майкрософт. Шифрование дополняет контроль доступа, защищая конфиденциальность контента клиента, где бы оно ни хранилось, и предотвращая чтение содержимого во время его перехода между системами Microsoft 365 или между Microsoft 365 и клиентом.

## <a name="how-does-microsoft-365-encrypt-data-at-rest"></a>Как Microsoft 365 шифрует неавтные данные?

Все содержимое клиента в Microsoft 365 защищено с помощью одной или более форм шифрования. Серверы Майкрософт используют BitLocker для шифрования дисков, содержащих содержимое клиента на уровне тома. Шифрование, предоставляемая BitLocker, защищает контент клиента в случае по иных процессов или элементов управления (например, управления доступом или перезапуска оборудования), что может привести к несанкционированному физическому доступу к дискам, содержащим контент клиента.

Exchange Online, Microsoft Teams, SharePoint Online и OneDrive для бизнеса также используют шифрование служб на уровне приложения для шифрования содержимого клиента. Шифрование служб предоставляет функции защиты прав и управления на основе сильной защиты шифрования. Это также позволяет разделять операционные системы Windows и данные клиента, хранимые или обрабатываемых этими операционными системами.

## <a name="how-does-microsoft-365-encrypt-data-in-transit"></a>Как Microsoft 365 шифрует данные при их передаче?

Продукты и службы Microsoft 365 используют протоколы транспорта, такие как TLS, для предотвращения перехвата несанкционированными сторонами данных клиентов во время их перемещения по сети. К примерам данных при передаче относятся почтовые сообщения, которые находятся в процессе доставки, беседы, происходящие в собрании по сети, или файлы, реплицируемые между центрами обработки данных.

В Microsoft 365 данные считаются "в пути" всякий раз, когда устройство пользователя общается с сервером Майкрософт или сервер Майкрософт общается с другим сервером. Exchange Online, SharePoint Online, Microsoft Teams и Office Online используют TLS, чтобы обеспечить конфиденциальность данных во время передачи.

## <a name="how-does-microsoft-365-manage-the-keys-used-for-encryption"></a>Как Microsoft 365 управляет ключами, используемыми для шифрования?

Надежное шифрование так же безопасно, как ключи, используемые для шифрования данных. Корпорация Майкрософт использует собственные сертификаты безопасности для шифрования подключений TLS для передачи данных. Для неавторных данных тома, защищенные BitLocker, шифруются с помощью ключа шифрования полного тома, который шифруется с помощью ключа тома, который, в свою очередь, привязан к доверенного платформенного модуля (TPM) на сервере. BitLocker использует алгоритмы, совместимые с FIPS, чтобы ключи шифрования никогда не хранились и не отправлялись по сети в зашифровки.

Шифрование службы обеспечивает дополнительный уровень шифрования данных клиентов в Exchange Online, Microsoft Teams, SharePoint Online и OneDrive для бизнеса. Шифрование службы предоставляет клиентам два варианта управления ключами шифрования: ключи под управлением Майкрософт или ключ клиента. При использовании ключей под управлением Майкрософт службы Microsoft 365 автоматически создают и безопасно сохраняют корневые ключи, используемые для шифрования служб.

Клиенты с требованиями для управления собственными корневыми ключами шифрования могут использовать шифрование службы с ключом клиента. С помощью ключа клиента клиенты могут создавать собственные криптографические ключи с помощью локального модуля аппаратного обслуживания (HSM) или Azure Key Vault (AKV). Корневые ключи клиента хранятся в AKV, где их можно использовать в качестве корня одной из ключевых фигур, шифруя данных или файлов почтовых ящиков клиентов. Код службы Microsoft 365 может получить доступ к корневым ключам клиента только опосредованно для шифрования данных и не может получить прямой доступ со стороны сотрудников Майкрософт.

## <a name="related-external-regulations--certifications"></a>Связанные внешние нормативы & сертификации

Веб-службы Майкрософт регулярно проверяются на соответствие внешним нормативным требованиям и сертификациям. Проверка элементов управления, связанных с шифрованием и управлением ключами, приводится в следующей таблице.

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365)](https://compliance.microsoft.com/compliancemanager) | SC-8: конфиденциальность и целостность передачи <br> SC-13: использование криптографии <br> SC-28: защита неавтной информации <br>  | 24 сентября 2020 г. |
| [ISO 27001/27002 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Заявление о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.10.1: криптографические элементы управления <br> A.18.1.5: криптографические элементы управления | 22 февраля 2020 г. |
| [ISO 27017 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Заявление о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.10.1: криптографические элементы управления <br> A.18.1.5: криптографические элементы управления | 22 февраля 2020 г. |
| [ISO 27018 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Заявление о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=43e89534-f48d-42ea-a7a7-3523ff516036&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.11.6. Шифрование личные сведения, передаваемые по общедоступным сетям передачи данных | 22 февраля 2020 г. |
| [SOC 2 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-44: шифрование при передаче данных <br> CA-54: шифрование неавтовых данных <br> CA-62: шифрование почтовых ящиков с ключом клиента <br> CA-63: удаление данных ключа клиента <br> CA-64: ключ клиента | 24 декабря 2020 г. |
| [SOC 3 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-16: ключи шифрования клиента <br> CUEC-17: хранилище ключей клиента <br>  CUEC-18: ротация ключей клиента| 24 декабря 2020 г. |
