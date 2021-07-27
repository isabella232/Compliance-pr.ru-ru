---
title: Microsoft 365 Yammer управления корпоративным доступом
description: В этой статье содержится краткое описание Yammer корпоративный элементов управления доступом в производственной среде.
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
- MS-Compliance
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: ac02d8ba8719d9ef78a24bee37732007af7cba8b
ms.sourcegitcommit: 07578a8e03b931f47c49f4e34b78cf8ba0605e8f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2021
ms.locfileid: "53573577"
---
# <a name="yammer-enterprise-access-controls"></a>Yammer элементов управления корпоративным доступом 

Физический и логический доступ к Yammer производственной среде ограничен небольшим набором людей (инфраструктура и операции). Как и другие Microsoft 365 инженеры, Yammer имеют нулевой постоянный доступ к данным клиентов. Доступ необходимо запрашивать с помощью системы управления доступом на основе утверждения, аналогичной lockbox с ограниченным числом утверждений. Утверждения проверяют запрос (например, проверяют, является ли запрос законным в зависимости от необходимости, бизнес-дела, времени и т.д.), а затем одобряют или отказывают в запросе. Если запрос утвержден, JIT-доступ предоставляется в течение определенного и ограниченного времени. После превышения времени доступа доступ автоматически истекает.

Как и в Microsoft 365 других службах, весь доступ к Yammer производственной среде использует многофакторную проверку подлинности. Вся история доступа и команд приписывается пользователю и регулярно регистрируется Yammer безопасности.

Дополнительные сведения об администрировании Yammer и управлении см. в Yammer [справке администратора.](/yammer/yammer-landing-page)