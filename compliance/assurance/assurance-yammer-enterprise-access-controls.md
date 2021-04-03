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
# <a name="yammer-enterprise-access-controls"></a><span data-ttu-id="3de5c-103">Элементы управления корпоративным доступом Yammer</span><span class="sxs-lookup"><span data-stu-id="3de5c-103">Yammer enterprise access controls</span></span> 

<span data-ttu-id="3de5c-104">Физический и логический доступ к среде производства Yammer ограничен небольшим набором людей (инфраструктура и операции).</span><span class="sxs-lookup"><span data-stu-id="3de5c-104">Physical and logical access to the Yammer production environment is restricted to a small set of people (infrastructure and operations).</span></span> <span data-ttu-id="3de5c-105">Как и другие инженеры Microsoft 365, инженеры Yammer имеют нулевой постоянный доступ к данным клиентов.</span><span class="sxs-lookup"><span data-stu-id="3de5c-105">As with other Microsoft 365 engineers, Yammer engineers have zero standing access to customer data.</span></span> <span data-ttu-id="3de5c-106">Доступ необходимо запрашивать с помощью системы управления доступом на основе утверждения, аналогичной lockbox с ограниченным числом утверждений.</span><span class="sxs-lookup"><span data-stu-id="3de5c-106">Access must be requested using an approval-based just-in-time access control system similar to Lockbox with a limited number of approvers.</span></span> <span data-ttu-id="3de5c-107">Утверждения проверяют запрос (например, проверяют, является ли запрос законным в зависимости от необходимости, бизнес-дела, времени и т.д.), а затем одобряют или отказывают в запросе.</span><span class="sxs-lookup"><span data-stu-id="3de5c-107">Approvers verify the request (for example, they verify whether the request is legitimate based on need, business case, time, etc.), and then approve or deny the request.</span></span> <span data-ttu-id="3de5c-108">Если запрос утвержден, JIT-доступ предоставляется в течение определенного и ограниченного времени.</span><span class="sxs-lookup"><span data-stu-id="3de5c-108">If the request is approved, JIT access is granted for a defined and limited time.</span></span> <span data-ttu-id="3de5c-109">После превышения времени доступа доступ автоматически истекает.</span><span class="sxs-lookup"><span data-stu-id="3de5c-109">After access time is exceeded, the access automatically expires.</span></span>

<span data-ttu-id="3de5c-110">Как и в других службах Microsoft 365, весь доступ к среде производства Yammer использует многофакторную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="3de5c-110">As with other Microsoft 365 services, all access to the Yammer production environment uses multi-factor authentication.</span></span> <span data-ttu-id="3de5c-111">Вся история доступа и команд приписывается пользователю и регулярно регистрируется и просматривается командой безопасности Yammer.</span><span class="sxs-lookup"><span data-stu-id="3de5c-111">All access and command history is attributed to a user, and logged and reviewed regularly by the Yammer security team.</span></span>

<span data-ttu-id="3de5c-112">Дополнительные сведения об администрировании и управлении Yammer см. в справке [по администрированию Yammer.](/yammer/yammer-landing-page)</span><span class="sxs-lookup"><span data-stu-id="3de5c-112">For more information about Yammer administration and management, see [Yammer admin help](/yammer/yammer-landing-page).</span></span>