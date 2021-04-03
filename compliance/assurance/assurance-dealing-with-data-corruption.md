---
title: Microsoft 365, занимаясь коррупцией данных
description: В этой статье объясняется коррупция данных в Microsoft 365 и усилия, предпринятые Корпорацией Майкрософт для предотвращения и восстановления данных.
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
ms.openlocfilehash: 9e9f0951f7e349cc70bc96bb6a2d62275848cf04
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51497593"
---
# <a name="dealing-with-data-corruption-in-microsoft-365"></a><span data-ttu-id="0441a-103">Борьба с коррупцией данных в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0441a-103">Dealing with data corruption in Microsoft 365</span></span>

<span data-ttu-id="0441a-104">Одним из сложных аспектов работы крупномасштабной облачной службы является обработка коррупции данных с учетом большого объема данных и независимых систем.</span><span class="sxs-lookup"><span data-stu-id="0441a-104">One of the challenging aspects of running a large-scale cloud service is how to handle data corruption, given the large volume of data and independent systems.</span></span> <span data-ttu-id="0441a-105">Коррупция данных может быть вызвана:</span><span class="sxs-lookup"><span data-stu-id="0441a-105">Data corruption can be caused by:</span></span>

- <span data-ttu-id="0441a-106">Ошибки приложения или инфраструктуры, развращающие часть или все состояние приложения</span><span class="sxs-lookup"><span data-stu-id="0441a-106">Application or infrastructure bugs, corrupting some or all of the application state</span></span>
- <span data-ttu-id="0441a-107">Проблемы с оборудованием, которые привели к потерям данных или невозможности чтения данных</span><span class="sxs-lookup"><span data-stu-id="0441a-107">Hardware issues that result in lost data or an inability to read data</span></span>
- <span data-ttu-id="0441a-108">Ошибки в работе человека</span><span class="sxs-lookup"><span data-stu-id="0441a-108">Human operational errors</span></span>
- <span data-ttu-id="0441a-109">Вредоносные хакеры и недовольные сотрудники</span><span class="sxs-lookup"><span data-stu-id="0441a-109">Malicious hackers and disgruntled employees</span></span>
- <span data-ttu-id="0441a-110">Инциденты во внешних службах, которые привели к некоторой потере данных</span><span class="sxs-lookup"><span data-stu-id="0441a-110">Incidents in external services that result in some loss of data</span></span>

<span data-ttu-id="0441a-111">Так как повышение устойчивости к целостности данных означает меньше инцидентов с повреждениями данных, Корпорация Майкрософт встроена в механизмы защиты Microsoft 365 для предотвращения коррупции, а также системы и процессы, которые позволяют восстановить данные, если это произойдет.</span><span class="sxs-lookup"><span data-stu-id="0441a-111">Because greater resiliency in data integrity means fewer data corruption incidents, Microsoft has built into Microsoft 365 protection mechanisms to prevent corruption from happening, as well as systems and processes that enable us to recover data if it does.</span></span> <span data-ttu-id="0441a-112">Проверки и процессы существуют на различных этапах процесса выпуска инженерных данных для повышения устойчивости к повреждениям данных, в том числе:</span><span class="sxs-lookup"><span data-stu-id="0441a-112">Checks and processes exist within the various stages of the engineering release process to increase resiliency against data corruption, including:</span></span>

- <span data-ttu-id="0441a-113">Проектирование системы</span><span class="sxs-lookup"><span data-stu-id="0441a-113">System Design</span></span>
- <span data-ttu-id="0441a-114">Организация и структура кода</span><span class="sxs-lookup"><span data-stu-id="0441a-114">Code organization and structure</span></span>
- <span data-ttu-id="0441a-115">Проверка кода</span><span class="sxs-lookup"><span data-stu-id="0441a-115">Code review</span></span>
- <span data-ttu-id="0441a-116">Unit tests, integration tests and system tests</span><span class="sxs-lookup"><span data-stu-id="0441a-116">Unit tests, integration tests, and system tests</span></span>
- <span data-ttu-id="0441a-117">Trip wires tests/gates</span><span class="sxs-lookup"><span data-stu-id="0441a-117">Trip wires tests/gates</span></span>

<span data-ttu-id="0441a-118">В производственных средах Microsoft 365 одноранговая репликация между центрами обработки данных гарантирует, что всегда существует несколько живых копий любых данных.</span><span class="sxs-lookup"><span data-stu-id="0441a-118">Within Microsoft 365 production environments, peer replication between datacenters ensures that there are always multiple live copies of any data.</span></span> <span data-ttu-id="0441a-119">Стандартные изображения и сценарии используются для восстановления потерянных серверов, а реплицированные данные используются для восстановления данных клиентов.</span><span class="sxs-lookup"><span data-stu-id="0441a-119">Standard images and scripts are used to recover lost servers, and replicated data is used to restore customer data.</span></span> <span data-ttu-id="0441a-120">Благодаря встроенным проверкам и процессам устойчивости к данным Корпорация Майкрософт поддерживает резервное копирование только документации информационной системы Microsoft 365 (включая документацию, связанную с безопасностью), используя встроенную репликацию в SharePoint Online и наш внутренний инструмент репозитория кода Source Depot.</span><span class="sxs-lookup"><span data-stu-id="0441a-120">Because of the built-in data resiliency checks and processes, Microsoft maintains backups only of Microsoft 365 information system documentation (including security-related documentation), using built-in replication in SharePoint Online and our internal code repository tool, Source Depot.</span></span> <span data-ttu-id="0441a-121">Документация по системе хранится в SharePoint Online, а Source Depot содержит изображения систем и приложений.</span><span class="sxs-lookup"><span data-stu-id="0441a-121">System documentation is stored in SharePoint Online, and Source Depot contains system and application images.</span></span> <span data-ttu-id="0441a-122">И SharePoint Online, и Source Depot используют версии и реплицированы в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="0441a-122">Both SharePoint Online and Source Depot use versioning and are replicated in near real time.</span></span>
