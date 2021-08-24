---
title: Microsoft 365 Ограничения ресурсов
description: В этой статье вы можете найти сведения об ограничениях ресурсов для различных приложений в Microsoft 365.
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
search.appverid:
- MET150
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 764259e22b23ecc7cea363283fc313a94875a2d1
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/23/2021
ms.locfileid: "58481791"
---
# <a name="service-resource-limits"></a>Ограничения ресурсов служб

Ограничения ресурсов применяются с помощью квот (ограничений) и регулирования. Azure Active Directory (Azure AD) и отдельные Microsoft 365 службы используют оба. Ограничения специфичен для служб и изменяются со временем при добавлении новых возможностей. Подробные сведения о текущих ограничениях для различных служб см. в следующих темах:

- [Ограничения и ограничения служб Azure AD](/azure/azure-resource-manager/management/azure-subscription-service-limits)
- [Ограничения Exchange Online](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)
- [SharePoint Границы и ограничения программного обеспечения в Интернете](https://support.office.com/article/SharePoint-Online-software-boundaries-and-limits-8F34FF47-B749-408B-ABC0-B605E1F6D498)
- [Skype для бизнеса Ограничения](https://technet.microsoft.com/library/skype-for-business-online-limits.aspx)
- [Yammer API REST и ограничения скорости](https://developer.yammer.com/docs/rest-api-rate-limits)
- [Ограничения размера файла в Sway](https://support.office.com/article/File-size-limits-in-Sway-4db21bc6-b42b-499f-9272-66e089db109f)

Помимо этих ограничений, в Azure AD и Microsoft 365 используются несколько механизмов регулирования. Регулирование в службе особенно важно, учитывая, что сетевые ресурсы в центрах обработки данных Майкрософт оптимизированы для широкого круга клиентов, которые используют эти службы. Механизмы регулирования включают:

- Azure AD и Microsoft 365 функции регулирования на уровне пользователя, которые ограничивают количество транзакций или одновредных вызовов (по сценарию или коду), которые могут выполняться одним пользователем.
- Политика регулирования PowerShell по умолчанию назначена каждому клиенту при создании клиента. Эти параметры влияют на другие элементы, например максимальное количество сеансов PowerShell, которые может открыть один администратор.
- Каждый Exchange Online по умолчанию имеет политику Exchange веб-служб (EWS), настроенную для клиентских операций EWS, и регулирование, которое применяется ко всем Outlook клиентам.
