---
title: Элементы управления корпоративным доступом Microsoft 365 Yammer
description: В этой статье содержится краткое описание элементов управления корпоративным доступом Yammer в производственной среде.
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
ms.openlocfilehash: df345d922bbd0c9106cf0714377803a9c0870d82
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51497356"
---
# <a name="yammer-enterprise-access-controls"></a>Элементы управления корпоративным доступом Yammer 

Физический и логический доступ к среде производства Yammer ограничен небольшим набором людей (инфраструктура и операции). Как и другие инженеры Microsoft 365, инженеры Yammer имеют нулевой постоянный доступ к данным клиентов. Доступ необходимо запрашивать с помощью системы управления доступом на основе утверждения, аналогичной lockbox с ограниченным числом утверждений. Утверждения проверяют запрос (например, проверяют, является ли запрос законным в зависимости от необходимости, бизнес-дела, времени и т.д.), а затем одобряют или отказывают в запросе. Если запрос утвержден, JIT-доступ предоставляется в течение определенного и ограниченного времени. После превышения времени доступа доступ автоматически истекает.

Как и в других службах Microsoft 365, весь доступ к среде производства Yammer использует многофакторную проверку подлинности. Вся история доступа и команд приписывается пользователю и регулярно регистрируется и просматривается командой безопасности Yammer.

Дополнительные сведения об администрировании и управлении Yammer см. в справке [по администрированию Yammer.](/yammer/yammer-landing-page)