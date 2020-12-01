---
title: Элементы управления доступом к Microsoft 365 Yammer корпоративный
description: В этой статье представлен краткий обзор элементов управления корпоративным доступом в Yammer в рабочей среде.
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
ms.openlocfilehash: d44bead3627ed9b99c93bcffc9f29f87731f7407
ms.sourcegitcommit: 626b0076d133e588cd28598c149a7f272fc18bae
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2020
ms.locfileid: "49508403"
---
# <a name="yammer-enterprise-access-controls"></a>Элементы управления корпоративным доступом в Yammer 

Физический и логический доступ к рабочей среде Yammer ограничена небольшим набором людей (инфраструктура и операции). Как и другие инженеры Microsoft 365, у специалистов Yammer есть нулевой доступ к данным клиента. Доступ должен быть запрошен с помощью системы управления доступом на основе утверждений, как и для защищенного хранилища, с ограниченным количеством утверждающих. Утверждающие проверяют запрос (например, проверяют, является ли запрос действительным на основании потребностей, Бизнес-дел, времени и т. д.), а затем Утвердите или отклоните запрос. Если запрос утвержден, JIT-доступ предоставляется для определенного и ограниченного времени. После превышения времени доступа срок действия доступа истекает автоматически.

Как и в случае с другими службами Microsoft 365, все доступ к рабочей среде Yammer использует многофакторную проверку подлинности. Все пользователи получают доступ к журналу команд и записываются в журнал и регулярно проверяются группой безопасности Yammer.

Для получения дополнительных сведений об администрировании и управлении Yammer обратитесь к [справочной статье администратора Yammer](https://docs.microsoft.com/yammer/yammer-landing-page).