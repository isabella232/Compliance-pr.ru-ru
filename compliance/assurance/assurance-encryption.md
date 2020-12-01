---
title: Обзор шифрования и управления ключами
description: Сведения о шифровании и управлении ключами в Microsoft 365
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
ms.openlocfilehash: 96a3871657dc1e6021949ca9fc2376df382fe15b
ms.sourcegitcommit: 626b0076d133e588cd28598c149a7f272fc18bae
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2020
ms.locfileid: "49508201"
---
# <a name="encryption-and-key-management-overview"></a>Обзор шифрования и управления ключами

## <a name="what-role-does-encryption-play-in-protecting-customer-content"></a>Какую роль выполняет шифрование при защите контента клиента?

Большинство облачных служб Microsoft Business являются многоклиентским, то есть контент клиентов может храниться на том же физическом оборудовании, что и другие клиенты. Чтобы защитить конфиденциальность контента клиента, Microsoft 365 шифрует все данные на месте и в транзите с использованием некоторых наиболее надежных и наиболее надежных протоколов шифрования.

Шифрование не является заменой строгих элементов управления доступом. Политика контроля доступа Microsoft 365 с нулевым доступом (ЗСА) защищает содержимое клиентов от несанкционированного доступа сотрудников Майкрософт. Шифрование дополняет управление доступом, защищая Конфиденциальность контента клиента везде, где он хранится, и предотвращения считывания содержимого в транзитном периоде между системами Microsoft 365 или Microsoft 365 и клиентом.

## <a name="how-does-microsoft-365-encrypt-data-at-rest"></a>Как Microsoft 365 шифрует данные — на других?

Все содержимое клиента в Microsoft 365 защищено одной или несколькими формами шифрования. Microsoft Servers использует BitLocker для шифрования дисков с контентом клиентов на уровне тома. Шифрование BitLocker обеспечивает защиту контента клиента в случае промежутков в других процессах или элементах управления (например, для управления доступом и повторного использования оборудования), которые могут привести к несанкционированному физическому доступу к дискам с контентом клиента.

Exchange Online, Microsoft Teams, SharePoint Online и OneDrive для бизнеса также используют шифрование служб на уровне приложений для шифрования контента клиента. Шифрование службы обеспечивает защиту и функции управления правами на основе надежной защиты шифрования. Он также позволяет разделить операционные системы Windows и данные клиентов, хранящиеся или обрабатываемые этими операционными системами.

## <a name="how-does-microsoft-365-encrypt-data-in-transit"></a>Как Microsoft 365 шифрует транзитный транзитный объем данных?

Продукты и службы Microsoft 365 используют надежные транспортные протоколы, такие как TLS, для предотвращения несанкционированного прослушивания данных клиентов при перемещении по сети. Примеры передаваемых данных включают почтовые сообщения, которые находятся в процессе доставки, беседы, выполняемые в собрании по сети, или файлы, реплицируемые между центрами обработки данных.

В Microsoft 365 данные считаются "транзитными", когда устройство пользователя обменивается данными с сервером Microsoft или сервер Microsoft взаимодействует с другим сервером. Exchange Online, SharePoint Online, Microsoft Teams и Office Online ALL используют протокол TLS для обеспечения конфиденциальности данных при передаче.

## <a name="how-does-microsoft-365-manage-the-keys-used-for-encryption"></a>Как Microsoft 365 управляет ключами, используемыми для шифрования?

Строгое шифрование применяется только для защиты ключей, используемых для шифрования данных. Корпорация Майкрософт использует собственные сертификаты безопасности, чтобы шифровать подключения TLS для транзитных данных. Тома, защищенные с помощью BitLocker, шифруются с помощью полного ключа шифрования тома, который в свою очередь связан с главным ключом тома, который, в свою очередь, связан с доверенным платформенным модулем на сервере. BitLocker использует алгоритмы, совместимые с FIPS, чтобы убедиться, что ключи шифрования никогда не хранятся и не отправляются по каналу в Clear.

Шифрование службы обеспечивает дополнительный уровень шифрования данных о клиентах в Exchange Online, Microsoft Teams, SharePoint Online и OneDrive для бизнеса. Шифрование службы предоставляет пользователям два варианта управления ключами шифрования: ключи, управляемые корпорацией Майкрософт, или ключ клиента. При использовании ключей, управляемых Майкрософт, службы Microsoft 365 автоматически создают и надежно сохраняют корневые ключи, используемые для шифрования службы.

Клиенты с требованиями для управления собственными корневыми ключами шифрования могут использовать шифрование службы с ключом клиента. С помощью ключа клиента клиенты могут создавать собственные криптографические ключи с помощью локального модуля службы оборудования (HSM) или Azure Key Vault (АКВ). Корневые ключи клиентов хранятся в АКВ, где их можно использовать в качестве корня одного из кэйчаинс, который шифрует данные или файлы почтового ящика клиента. Доступ к корневым ключам клиентов возможен только непосредственно с помощью кода службы Microsoft 365 для шифрования данных и недоступен для сотрудников Майкрософт.

## <a name="related-external-regulations--certifications"></a>Связанные внешние нормативные & сертификации

Веб-службы корпорации Майкрософт регулярно подлежат аудиту для соответствия внешним нормативам и сертификациям. В следующей таблице приведены сведения о проверке элементов управления, связанных с шифрованием и управлением ключами.

| **Внешние аудиты** | **Section** | **Дата последнего отчета** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365)](https://compliance.microsoft.com/compliancemanager) | SC – 8: конфиденциальность и целостность передачи <br> SC – 13: использование шифрования <br> SC – 28: защита данных на REST <br>  | 24 сентября 2020 г. |
| [ISO 27001/27002 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Отчет о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A. 10.1: криптографические элементы управления <br> A. 18.1.5: криптографические элементы управления | 22 февраля 2020 г. |
| [ISO 27017 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Отчет о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A. 10.1: криптографические элементы управления <br> A. 18.1.5: криптографические элементы управления | 22 февраля 2020 г. |
| [ISO 27018 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Отчет о применимости](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Сертификация](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=43e89534-f48d-42ea-a7a7-3523ff516036&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A. 11.6: шифрование личных данных, передаваемых через общедоступные сети передачи данных | 22 февраля 2020 г. |
| [SOC 2 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=fa062990-e758-4ddc-ace3-7fb21a301d09&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Rep-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Reports) | CA — 44: шифрование данных в транзитном месте <br> CA — 54: шифрование данных на REST <br> CA — 62: шифрование клиентского почтового ящика <br> CA — 63: удаление данных ключа клиента <br> CA — 64: ключ клиента | 30 сентября 2019 г. |
| [SOC 3 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=9df8b99b-96ce-49a9-bff4-268031dcc9a6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Reports) | КУЕК – 16: ключи шифрования клиентов <br> КУЕК – 17: хранилище ключей клиентов <br>  КУЕК – 18: ключевой цикл клиента| 30 сентября 2019 г. |
