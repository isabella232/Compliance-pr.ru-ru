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
# <a name="encryption-for-data-in-transit"></a><span data-ttu-id="04e91-103">Шифрование для передачи данных</span><span class="sxs-lookup"><span data-stu-id="04e91-103">Encryption for data-in-transit</span></span>

<span data-ttu-id="04e91-104">Помимо защиты данных клиентов в покое Корпорация Майкрософт использует технологии шифрования для защиты данных клиентов при транзите.</span><span class="sxs-lookup"><span data-stu-id="04e91-104">In addition to protecting customer data at rest, Microsoft uses encryption technologies to protect customer data in transit.</span></span> <span data-ttu-id="04e91-105">Данные в пути:</span><span class="sxs-lookup"><span data-stu-id="04e91-105">Data is in transit:</span></span>

- <span data-ttu-id="04e91-106">когда клиентская машина взаимодействует с сервером Майкрософт;</span><span class="sxs-lookup"><span data-stu-id="04e91-106">when a client machine communicates with a Microsoft server;</span></span>
- <span data-ttu-id="04e91-107">когда сервер Майкрософт взаимодействует с другим сервером Майкрософт; и</span><span class="sxs-lookup"><span data-stu-id="04e91-107">when a Microsoft server communicates with another Microsoft server; and</span></span>
- <span data-ttu-id="04e91-108">когда сервер Майкрософт взаимодействует с не microsoft server (например, Exchange Online доставляет электронную почту на сторонний сервер электронной почты).</span><span class="sxs-lookup"><span data-stu-id="04e91-108">when a Microsoft server communicates with a non-Microsoft server (for example, Exchange Online delivering email to a third-party email server).</span></span>

<span data-ttu-id="04e91-109">Междоусобные связи между серверами Майкрософт проходят через TLS или IPsec, и все серверы, стоящие перед клиентами, ведут переговоры о безопасном сеансе с использованием TLS с клиентской машиной (например, Exchange Online использует TLS 1.2 с 256-битной шифровкой( FIPS 140-2 Level 2-validated).</span><span class="sxs-lookup"><span data-stu-id="04e91-109">Inter-data center communications between Microsoft servers take place over TLS or IPsec, and all customer-facing servers negotiate a secure session using TLS with client machines (for example, Exchange Online uses TLS 1.2 with 256-bit cipher strength is used (FIPS 140-2 Level 2-validated).</span></span> <span data-ttu-id="04e91-110">[(См. технические справочные сведения о](/microsoft-365/compliance/technical-reference-details-about-encryption) шифровании для списка шифров TLS-пакетов, поддерживаемых Office 365.) Это относится к протоколам, используемым клиентами, такими как Outlook, Skype для бизнеса, Microsoft Teams и Outlook в Интернете (например, HTTP, POP3 и т.д.).</span><span class="sxs-lookup"><span data-stu-id="04e91-110">(See [Technical reference details about encryption](/microsoft-365/compliance/technical-reference-details-about-encryption) for a list of TLS cipher suites supported by Office 365.) This applies to the protocols that are used by clients such as Outlook, Skype for Business, Microsoft Teams, and Outlook on the web (for example, HTTP, POP3, etc.).</span></span>

<span data-ttu-id="04e91-111">Общедоступные сертификаты выдаются корпорацией Майкрософт ИТ-SSL с помощью SSLAdmin, внутреннего средства Майкрософт для защиты конфиденциальности передаваемых сведений.</span><span class="sxs-lookup"><span data-stu-id="04e91-111">The public certificates are issued by Microsoft IT SSL using SSLAdmin, an internal Microsoft tool to protect confidentiality of transmitted information.</span></span> <span data-ttu-id="04e91-112">Все сертификаты, выдавлимые корпорацией Майкрософт, имеют не менее 2048 битов в длину, а для соответствия требованиям веб-сайта требуется SSLAdmin, чтобы убедиться, что сертификаты выданы только общедоступным IP-адресам, которые принадлежат Корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="04e91-112">All certificates issued by Microsoft IT have a minimum of 2048 bits in length, and Webtrust compliance requires SSLAdmin to make sure that certificates are issued only to public IP addresses owned by Microsoft.</span></span> <span data-ttu-id="04e91-113">Все IP-адреса, которые не соответствуют этому критерию, проходят через процесс исключения.</span><span class="sxs-lookup"><span data-stu-id="04e91-113">Any IP addresses that fail to meet this criterion are routed through an exception process.</span></span>

<span data-ttu-id="04e91-114">Все сведения о реализации, такие как используемая версия TLS, включена ли форвардная секретность (FS), порядок наборов шифров и т. д., доступны публично.</span><span class="sxs-lookup"><span data-stu-id="04e91-114">All implementation details such as the version of TLS being used, whether Forward Secrecy (FS) is enabled, the order of cipher suites, etc., are available publicly.</span></span> <span data-ttu-id="04e91-115">Один из способов увидеть эти сведения — использовать сторонний веб-сайт, например [Qualys SSL Labs.](https://www.ssllabs.com)</span><span class="sxs-lookup"><span data-stu-id="04e91-115">One way to see these details is to use a third-party website, such as [Qualys SSL Labs](https://www.ssllabs.com).</span></span> <span data-ttu-id="04e91-116">Ниже приведены ссылки на автоматические тестовые страницы qualys, на которые отображаются сведения для следующих служб:</span><span class="sxs-lookup"><span data-stu-id="04e91-116">Below are the links to automated test pages from Qualys that display information for the following services:</span></span>

- [<span data-ttu-id="04e91-117">Портал Office 365</span><span class="sxs-lookup"><span data-stu-id="04e91-117">Office 365 Portal</span></span>](https://www.ssllabs.com/ssltest/analyze.html?d=portal.office.com&hideResults=on)
- [<span data-ttu-id="04e91-118">Exchange Online</span><span class="sxs-lookup"><span data-stu-id="04e91-118">Exchange Online</span></span>](https://www.ssllabs.com/ssltest/analyze.html?d=outlook.office365.com&hideResults=on)
- [<span data-ttu-id="04e91-119">SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="04e91-119">SharePoint Online</span></span>](https://www.ssllabs.com/ssltest/analyze.html?d=microsoft-my.sharepoint.com&hideResults=on)
- [<span data-ttu-id="04e91-120">Skype для бизнеса (SIP)</span><span class="sxs-lookup"><span data-stu-id="04e91-120">Skype for Business (SIP)</span></span>](https://www.ssllabs.com/ssltest/analyze.html?d=sipdir.online.lync.com)
- [<span data-ttu-id="04e91-121">Skype для бизнеса (Веб)</span><span class="sxs-lookup"><span data-stu-id="04e91-121">Skype for Business (Web)</span></span>](https://www.ssllabs.com/ssltest/analyze.html?d=webdir.online.lync.com&hideResults=on)
- [<span data-ttu-id="04e91-122">Exchange Online Protection</span><span class="sxs-lookup"><span data-stu-id="04e91-122">Exchange Online Protection</span></span>](https://ssl-tools.net/mailservers/microsoft-com.mail.protection.outlook.com)
- [<span data-ttu-id="04e91-123">Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="04e91-123">Microsoft Teams</span></span>](https://www.ssllabs.com/ssltest/analyze.html?d=teams.microsoft.com&latest)

<span data-ttu-id="04e91-124">Для Exchange Online Protection URL-адреса различаются по именам клиентов; однако все клиенты могут протестировать Microsoft 365 с **microsoft-com.mail.protection.outlook.com**.</span><span class="sxs-lookup"><span data-stu-id="04e91-124">For Exchange Online Protection, URLs vary by tenant names; however, all customers can test Microsoft 365 using **microsoft-com.mail.protection.outlook.com**.</span></span>
