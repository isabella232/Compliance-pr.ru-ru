---
title: Ограничения ресурсов Microsoft 365
description: В этой статье вы можете найти сведения об ограничениях ресурсов для различных приложений в Microsoft 365.
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
hideEdit: true
ms.openlocfilehash: 54ea001e542cdd1ab078546cf96bd011e27ab1dc
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51497498"
---
# <a name="service-resource-limits"></a>Ограничения ресурсов служб

Ограничения ресурсов применяются с помощью квот (ограничений) и регулирования. Azure Active Directory (Azure AD) и отдельные службы Microsoft 365 используют обе службы. Ограничения специфичен для служб и изменяются со временем при добавлении новых возможностей. Подробные сведения о текущих ограничениях для различных служб см. в следующих темах:

- [Ограничения и ограничения служб Azure AD](/azure/azure-resource-manager/management/azure-subscription-service-limits)
- [Ограничения Exchange Online](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)
- [Границы и ограничения программного обеспечения SharePoint Online](https://support.office.com/article/SharePoint-Online-software-boundaries-and-limits-8F34FF47-B749-408B-ABC0-B605E1F6D498)
- [Ограничения Skype для бизнеса](https://technet.microsoft.com/library/skype-for-business-online-limits.aspx)
- [API REST Yammer и ограничения скорости](https://developer.yammer.com/docs/rest-api-rate-limits)
- [Ограничения размера файла в Sway](https://support.office.com/article/File-size-limits-in-Sway-4db21bc6-b42b-499f-9272-66e089db109f)

Помимо этих ограничений, в Azure AD и Microsoft 365 используются несколько механизмов регулирования. Регулирование в службе особенно важно, учитывая, что сетевые ресурсы в центрах обработки данных Майкрософт оптимизированы для широкого круга клиентов, которые используют эти службы. Механизмы регулирования включают:

- Azure AD и Microsoft 365 имеют функции регулирования на уровне пользователей, которые ограничивают количество транзакций или одновредных вызовов (по сценарию или коду), которые могут выполняться одним пользователем.
- Политика регулирования PowerShell по умолчанию назначена каждому клиенту при создании клиента. Эти параметры влияют на другие элементы, например максимальное количество сеансов PowerShell, которые может открыть один администратор.
- Каждый клиент Exchange Online имеет политику Exchange Web Services (EWS) по умолчанию, настроенную для клиентских операций EWS, и регулирование, которое применяется ко всем клиентам Outlook.
