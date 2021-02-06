---
title: Ограничения ресурсов Microsoft 365
description: В этой статье вы найдете сведения об ограничениях ресурсов для различных приложений в Microsoft 365.
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: Normal
search.appverid:
- MET150
ms.collection:
- Strat_O365_IP
- M365-security-compliance
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: 632a0b78c5c5ba02a59f8863c2e751f009cc968e
ms.sourcegitcommit: 21ed42335efd37774ff5d17d9586d5546147241a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2021
ms.locfileid: "50120758"
---
# <a name="service-resource-limits"></a>Ограничения ресурсов служб

Ограничения ресурсов применяются с помощью квот (ограничений) и регулирования. Azure Active Directory (Azure AD) и отдельные службы Microsoft 365 используют обе службы. Ограничения специфичен для служб и со временем изменяются по мере того, как добавляются новые возможности. Сведения о текущих ограничениях для различных служб см. в следующих темах:

- [Ограничения для служб Azure AD](/azure/azure-resource-manager/management/azure-subscription-service-limits)
- [Ограничения Exchange Online](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)
- [Ограничения для программного обеспечения SharePoint Online](https://support.office.com/article/SharePoint-Online-software-boundaries-and-limits-8F34FF47-B749-408B-ABC0-B605E1F6D498)
- [Ограничения Skype для бизнеса](https://technet.microsoft.com/library/skype-for-business-online-limits.aspx)
- [Rest API Yammer и ограничения скорости](https://developer.yammer.com/docs/rest-api-rate-limits)
- [Ограничения на размер файлов в Sway](https://support.office.com/article/File-size-limits-in-Sway-4db21bc6-b42b-499f-9272-66e089db109f)

Помимо этих ограничений, в Azure AD и Microsoft 365 используется несколько механизмов регулирования. Регулирование в службе особенно важно, поскольку сетевые ресурсы в центрах обработки данных Майкрософт оптимизированы для широкого круга клиентов, которые используют службы. К механизмам регулирования относятся:

- Регулирование на уровне пользователя в Azure AD и Microsoft 365, ограничивающее количество транзакций или одновредных вызовов (по сценарию или коду), которые может выполнять один пользователь.
- Политика регулирования PowerShell по умолчанию назначена каждому арендатору при создании клиента. Эти параметры влияют на другие элементы, например максимальное количество одновременных сеансов PowerShell, которые может открыть один администратор.
- Каждый клиент Exchange Online имеет политику веб-служб Exchange (EWS) по умолчанию, настроенную для клиентских операций EWS, и регулирование, которое применяется ко всем клиентам Outlook.
