---
title: Шифрование для передачи данных
description: В этой статье найдите краткое объяснение того, как Microsoft Microsoft 365 данные клиентов в пути.
ms.author: krowley
author: kccross
manager: laurawi
ms.reviewer: sosstah
f1.keywords:
- NOCSH
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
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
ms.openlocfilehash: ebeface33b0d5ba419773c13305c277d681e8400
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59160091"
---
# <a name="encryption-for-data-in-transit"></a>Шифрование для передачи данных

Помимо защиты данных клиентов в покое Корпорация Майкрософт использует технологии шифрования для защиты данных клиентов при транзите. Данные в пути:

- когда клиентская машина взаимодействует с сервером Майкрософт;
- когда сервер Майкрософт взаимодействует с другим сервером Майкрософт; и
- когда сервер Майкрософт взаимодействует с не microsoft server (например, Exchange Online доставку электронной почты на сторонний сервер электронной почты).

Междоусобные связи между серверами Майкрософт проходят через TLS или IPsec, и все серверы, стоящие перед клиентом, ведут переговоры о безопасном сеансе с помощью TLS с клиентских машин (например, Exchange Online использует TLS 1.2 с 256-битной шифровкой (FIPS 140-2 Level 2-validated). [(См. технические справочные сведения о](/microsoft-365/compliance/technical-reference-details-about-encryption) шифровании для списка наборов шифров TLS, поддерживаемых Office 365.) Это относится к протоколам, используемым клиентами, такими как Outlook, Skype для бизнеса, Microsoft Teams и Outlook в Интернете (например, HTTP, POP3 и т.д.).

Общедоступные сертификаты выдаются корпорацией Майкрософт ИТ-SSL с помощью SSLAdmin, внутреннего средства Майкрософт для защиты конфиденциальности передаваемых сведений. Все сертификаты, выдавлимые корпорацией Майкрософт, имеют не менее 2048 битов в длину, а для соответствия требованиям веб-сайта требуется SSLAdmin, чтобы убедиться, что сертификаты выданы только общедоступным IP-адресам, которые принадлежат Корпорации Майкрософт. Все IP-адреса, которые не соответствуют этому критерию, проходят через процесс исключения.

Все сведения о реализации, такие как используемая версия TLS, включена ли форвардная секретность (FS), порядок наборов шифров и т. д., доступны публично. Один из способов увидеть эти сведения — использовать сторонний веб-сайт, например [Qualys SSL Labs.](https://www.ssllabs.com) Ниже приведены ссылки на автоматические тестовые страницы qualys, на которые отображаются сведения для следующих служб:

- [Office 365 Портал](https://www.ssllabs.com/ssltest/analyze.html?d=portal.office.com&hideResults=on)
- [Exchange Online](https://www.ssllabs.com/ssltest/analyze.html?d=outlook.office365.com&hideResults=on)
- [SharePoint Online](https://www.ssllabs.com/ssltest/analyze.html?d=microsoft-my.sharepoint.com&hideResults=on)
- [Skype для бизнеса (SIP)](https://www.ssllabs.com/ssltest/analyze.html?d=sipdir.online.lync.com)
- [Skype для бизнеса (Веб)](https://www.ssllabs.com/ssltest/analyze.html?d=webdir.online.lync.com&hideResults=on)
- [Exchange Online Protection](https://ssl-tools.net/mailservers/microsoft-com.mail.protection.outlook.com)
- [Microsoft Teams](https://www.ssllabs.com/ssltest/analyze.html?d=teams.microsoft.com&latest)

Для Exchange Online Protection URL-адреса различаются по именам клиентов; однако все клиенты могут протестировать Microsoft 365 с **помощью microsoft-com.mail.protection.outlook.com**.
