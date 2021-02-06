---
title: Шифрование для передачи данных
description: В этой статье вы найдете краткое описание того, как Майкрософт шифрует данные клиентов Microsoft 365 при их передаче.
ms.author: krowley
author: kccross
manager: laurawi
ms.reviewer: sosstah
f1.keywords:
- NOCSH
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: None
search.appverid:
- MET150
ms.collection:
- Strat_O365_Enterprise
- M365-security-compliance
- Strat_O365_Enterprise
- MS-Compliance
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: b6d6ae53ef2ade842e0e9205c01b44fe17891a97
ms.sourcegitcommit: 21ed42335efd37774ff5d17d9586d5546147241a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2021
ms.locfileid: "50120538"
---
# <a name="encryption-for-data-in-transit"></a>Шифрование для передачи данных

Помимо защиты неавтных данных клиентов Майкрософт использует технологии шифрования для защиты данных клиентов при передаче. Данные в пути:

- когда клиентский компьютер взаимодействует с сервером Майкрософт;
- когда сервер Майкрософт взаимодействует с другим сервером Майкрософт; и
- когда сервер Майкрософт взаимодействует с сервером, который не является сервером Майкрософт (например, Exchange Online доставляет электронную почту на сторонний почтовый сервер).

Связь между центрами обработки данных между серверами Майкрософт проходит через TLS или IPsec, и все клиентские серверы согласовыют безопасный сеанс с помощью TLS с клиентских компьютеров (например, Exchange Online использует TLS 1.2 с 256-битной степенью шифра (проверяется FIPS 140-2 уровня 2). [(См. технические справочные сведения о шифровании](/microsoft-365/compliance/technical-reference-details-about-encryption) для списка наборов шифров TLS, поддерживаемых Office 365.) Это относится к протоколам, используемым клиентами, такими как Outlook, Skype для бизнеса, Microsoft Teams и Outlook в Интернете (например, HTTP, POP3 и т. д.).

Общедоступные сертификаты выданы Microsoft IT SSL с помощью SSLAdmin, внутреннего средства Майкрософт для защиты конфиденциальности передаваемой информации. Длина всех сертификатов, выдавляемая ИТ-службой Майкрософт, не менее 2048 бит, а для обеспечения соответствия требованиям веб-структуры требуется SSLAdmin, чтобы убедиться, что сертификаты выданы только на общедоступные IP-адреса, которые принадлежат корпорации Майкрософт. Все IP-адреса, которые не соответствуют этому критерию, маршрутизации через процесс исключения.

Все сведения о реализации, такие как используемая версия TLS, включена ли forward Secrecy (FS), порядок наборов шифров и т. д., доступны в общедоступных целях. Один из способов увидеть эти сведения — использовать сторонний веб-сайт, например [Qualys SSL Labs.](https://www.ssllabs.com) Ниже приведены ссылки на автоматические тестовые страницы из Qualys, на которые отображаются сведения для следующих служб:

- [Портал Office 365](https://www.ssllabs.com/ssltest/analyze.html?d=portal.office.com&hideResults=on)
- [Exchange Online](https://www.ssllabs.com/ssltest/analyze.html?d=outlook.office365.com&hideResults=on)
- [SharePoint Online](https://www.ssllabs.com/ssltest/analyze.html?d=microsoft-my.sharepoint.com&hideResults=on)
- [Skype для бизнеса (SIP)](https://www.ssllabs.com/ssltest/analyze.html?d=sipdir.online.lync.com)
- [Skype для бизнеса (Интернет)](https://www.ssllabs.com/ssltest/analyze.html?d=webdir.online.lync.com&hideResults=on)
- [Exchange Online Protection](https://ssl-tools.net/mailservers/microsoft-com.mail.protection.outlook.com)
- [Microsoft Teams](https://www.ssllabs.com/ssltest/analyze.html?d=teams.microsoft.com&latest)

В Exchange Online Protection URL-адреса зависят от имен клиентов; однако все клиенты могут тестировать Microsoft 365 с **помощью microsoft-com.mail.protection.outlook.com.**
