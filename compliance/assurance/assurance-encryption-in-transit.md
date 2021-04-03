---
title: Шифрование для передачи данных
description: В этой статье вы найдете краткое объяснение того, как Microsoft шифрует данные клиентов Microsoft 365 при транзите.
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
hideEdit: true
ms.openlocfilehash: 227f74140ecd9b6283b92e8b0e87bd70912ec8e3
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51497253"
---
# <a name="encryption-for-data-in-transit"></a>Шифрование для передачи данных

Помимо защиты данных клиентов в покое Корпорация Майкрософт использует технологии шифрования для защиты данных клиентов при транзите. Данные в пути:

- когда клиентская машина взаимодействует с сервером Майкрософт;
- когда сервер Майкрософт взаимодействует с другим сервером Майкрософт; и
- когда сервер Майкрософт взаимодействует с не microsoft server (например, Exchange Online доставляет электронную почту на сторонний сервер электронной почты).

Междоусобные связи между серверами Майкрософт проходят через TLS или IPsec, и все серверы, стоящие перед клиентами, ведут переговоры о безопасном сеансе с использованием TLS с клиентской машиной (например, Exchange Online использует TLS 1.2 с 256-битной шифровкой( FIPS 140-2 Level 2-validated). [(См. технические справочные сведения о](/microsoft-365/compliance/technical-reference-details-about-encryption) шифровании для списка шифров TLS-пакетов, поддерживаемых Office 365.) Это относится к протоколам, используемым клиентами, такими как Outlook, Skype для бизнеса, Microsoft Teams и Outlook в Интернете (например, HTTP, POP3 и т.д.).

Общедоступные сертификаты выдаются корпорацией Майкрософт ИТ-SSL с помощью SSLAdmin, внутреннего средства Майкрософт для защиты конфиденциальности передаваемых сведений. Все сертификаты, выдавлимые корпорацией Майкрософт, имеют не менее 2048 битов в длину, а для соответствия требованиям веб-сайта требуется SSLAdmin, чтобы убедиться, что сертификаты выданы только общедоступным IP-адресам, которые принадлежат Корпорации Майкрософт. Все IP-адреса, которые не соответствуют этому критерию, проходят через процесс исключения.

Все сведения о реализации, такие как используемая версия TLS, включена ли форвардная секретность (FS), порядок наборов шифров и т. д., доступны публично. Один из способов увидеть эти сведения — использовать сторонний веб-сайт, например [Qualys SSL Labs.](https://www.ssllabs.com) Ниже приведены ссылки на автоматические тестовые страницы qualys, на которые отображаются сведения для следующих служб:

- [Портал Office 365](https://www.ssllabs.com/ssltest/analyze.html?d=portal.office.com&hideResults=on)
- [Exchange Online](https://www.ssllabs.com/ssltest/analyze.html?d=outlook.office365.com&hideResults=on)
- [SharePoint Online](https://www.ssllabs.com/ssltest/analyze.html?d=microsoft-my.sharepoint.com&hideResults=on)
- [Skype для бизнеса (SIP)](https://www.ssllabs.com/ssltest/analyze.html?d=sipdir.online.lync.com)
- [Skype для бизнеса (Веб)](https://www.ssllabs.com/ssltest/analyze.html?d=webdir.online.lync.com&hideResults=on)
- [Exchange Online Protection](https://ssl-tools.net/mailservers/microsoft-com.mail.protection.outlook.com)
- [Microsoft Teams](https://www.ssllabs.com/ssltest/analyze.html?d=teams.microsoft.com&latest)

Для Exchange Online Protection URL-адреса различаются по именам клиентов; однако все клиенты могут протестировать Microsoft 365 с **microsoft-com.mail.protection.outlook.com**.
