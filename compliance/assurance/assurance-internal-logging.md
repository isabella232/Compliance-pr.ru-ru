---
title: Microsoft 365 внутреннего ведения журнала для Microsoft 365 инженерии
description: В этой статье найдите объяснение того, как работает внутренний журнал для Microsoft 365 инженерных групп.
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
ms.openlocfilehash: 71b08509ae920ad88ecfa1566b9a11d640b0534f
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53088598"
---
# <a name="internal-logging-for-microsoft-365-engineering"></a><span data-ttu-id="fb1f4-103">Внутренняя регистрация для инженеров Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fb1f4-103">Internal logging for Microsoft 365 engineering</span></span>

<span data-ttu-id="fb1f4-104">Помимо событий и данных журналов, доступных для клиентов, Корпорация Майкрософт поддерживает внутреннюю систему сбора данных журналов, доступную Microsoft 365 инженерам.</span><span class="sxs-lookup"><span data-stu-id="fb1f4-104">In addition to the events and log data available for customers, Microsoft maintains an internal log data collection system that is available to Microsoft 365 engineers.</span></span> <span data-ttu-id="fb1f4-105">Многие типы данных журналов загружаются с Microsoft 365 серверов в несвободное решение мониторинга безопасности для анализа в режиме реального времени (NRT) и внутреннюю службу вычислений больших данных (Cosmos) для долгосрочного хранения.</span><span class="sxs-lookup"><span data-stu-id="fb1f4-105">Many different types of log data are uploaded from Microsoft 365 servers to a proprietary security monitoring solution for near real-time (NRT) analysis and an internal, big data computing service (Cosmos) for long-term storage.</span></span> <span data-ttu-id="fb1f4-106">Этот перенос данных происходит через подключение TLS с проверкой FIPS 140-2 в утвержденных портах и протоколах с помощью средства собственной автоматизации, называемого погрузчиком данных Office (ODL).</span><span class="sxs-lookup"><span data-stu-id="fb1f4-106">This data transfer occurs over a FIPS 140-2-validated TLS connection on approved ports and protocols using a proprietary automation tool called the Office Data Loader (ODL).</span></span> <span data-ttu-id="fb1f4-107">Средства, используемые в Microsoft 365 для сбора и обработки записей аудита, не позволяют вносить постоянные или необратимые изменения в исходное содержимое записи аудита или порядок времени.</span><span class="sxs-lookup"><span data-stu-id="fb1f4-107">The tools used in Microsoft 365 to collect and process audit records do not allow permanent or irreversible changes to the original audit record content or time ordering.</span></span>

<span data-ttu-id="fb1f4-108">Группы служб используют Cosmos как централизованный репозиторий для анализа использования приложений, измерения производительности системы и операционной деятельности, а также для проверки нарушений и шаблонов, которые могут указывать на проблемы или проблемы с безопасностью.</span><span class="sxs-lookup"><span data-stu-id="fb1f4-108">Service teams use Cosmos as a centralized repository to conduct an analysis of application usage, to measure system and operational performance, and to look for abnormalities and patterns that may indicate problems or security issues.</span></span> <span data-ttu-id="fb1f4-109">Каждая группа служб загружает базовый уровень, который включает в себя:</span><span class="sxs-lookup"><span data-stu-id="fb1f4-109">Each service team uploads a baseline that includes:</span></span>

- <span data-ttu-id="fb1f4-110">Журналы событий</span><span class="sxs-lookup"><span data-stu-id="fb1f4-110">Event logs</span></span>
- <span data-ttu-id="fb1f4-111">Журналы AppLocker</span><span class="sxs-lookup"><span data-stu-id="fb1f4-111">AppLocker logs</span></span>
- <span data-ttu-id="fb1f4-112">Данные о производительности</span><span class="sxs-lookup"><span data-stu-id="fb1f4-112">Performance data</span></span>
- <span data-ttu-id="fb1f4-113">System Center данных</span><span class="sxs-lookup"><span data-stu-id="fb1f4-113">System Center data</span></span>
- <span data-ttu-id="fb1f4-114">Записи детализации вызовов</span><span class="sxs-lookup"><span data-stu-id="fb1f4-114">Call detail records</span></span>
- <span data-ttu-id="fb1f4-115">Качество данных об опыте</span><span class="sxs-lookup"><span data-stu-id="fb1f4-115">Quality of experience data</span></span>
- <span data-ttu-id="fb1f4-116">Журналы веб-сервера IIS</span><span class="sxs-lookup"><span data-stu-id="fb1f4-116">IIS Web Server logs</span></span>
- <span data-ttu-id="fb1f4-117">SQL Server журналы</span><span class="sxs-lookup"><span data-stu-id="fb1f4-117">SQL Server logs</span></span>
- <span data-ttu-id="fb1f4-118">Данные Syslog</span><span class="sxs-lookup"><span data-stu-id="fb1f4-118">Syslog data</span></span>
- <span data-ttu-id="fb1f4-119">Журналы аудита безопасности</span><span class="sxs-lookup"><span data-stu-id="fb1f4-119">Security audit logs</span></span>

<span data-ttu-id="fb1f4-120">Перед отправкой приложение ODL использует службу очистки, чтобы удалить все поля, содержащие данные клиента, такие как сведения о клиентах и идентифицируемые конечными пользователями сведения, и заменить эти поля значением hash.</span><span class="sxs-lookup"><span data-stu-id="fb1f4-120">Prior to uploading, the ODL application uses a scrubbing service to remove any fields that contain customer data, such as tenant information and end-user identifiable information, and replace those fields with a hash value.</span></span> <span data-ttu-id="fb1f4-121">Вымытые журналы загружаются в Cosmos и в решение мониторинга безопасности NRT, которое анализирует журналы для потенциальных событий безопасности и показателей производительности.</span><span class="sxs-lookup"><span data-stu-id="fb1f4-121">The scrubbed logs are uploaded to Cosmos and to the NRT security monitoring solution that analyzes the logs for potential security events and performance indicators.</span></span> <span data-ttu-id="fb1f4-122">Период хранения данных журнала аудита в Cosmos определяется группами служб; большинство данных журнала аудита сохраняется в течение 90 дней или дольше для поддержки расследований инцидентов безопасности и для удовлетворения требований к хранению нормативных данных.</span><span class="sxs-lookup"><span data-stu-id="fb1f4-122">The period of audit log data retention in Cosmos is determined by the service teams; most audit log data is retained for 90 days or longer to support security incident investigations and to meet regulatory retention requirements.</span></span>

<span data-ttu-id="fb1f4-123">Доступ к Microsoft 365, хранимых в Cosmos, ограничен уполномоченным персоналом.</span><span class="sxs-lookup"><span data-stu-id="fb1f4-123">Access to Microsoft 365 data stored in Cosmos is restricted to authorized personnel.</span></span> <span data-ttu-id="fb1f4-124">Корпорация Майкрософт ограничивает управление журналами аудита ограниченным подмножеством членов группы безопасности, отвечающих за функции аудита.</span><span class="sxs-lookup"><span data-stu-id="fb1f4-124">Microsoft restricts the management of audit logs to a limited subset of Security Team members responsible for audit functionality.</span></span> <span data-ttu-id="fb1f4-125">Группа безопасности не имеет постоянного административного доступа к Cosmos, и все изменения записывают и проверяют.</span><span class="sxs-lookup"><span data-stu-id="fb1f4-125">The Security Team does not have standing administrative access to Cosmos, and all changes are recorded and audited.</span></span>

<span data-ttu-id="fb1f4-126">После анализа NRT каждая группа служб может использовать средства анализа и панели мониторинга для корреляции данных, интерактивных запросов и аналитики данных.</span><span class="sxs-lookup"><span data-stu-id="fb1f4-126">After NRT analysis, each service team can use analysis tools and dashboards for data correlation, interactive queries, and data analytics.</span></span> <span data-ttu-id="fb1f4-127">Эти отчеты используются для мониторинга и повышения общей производительности службы.</span><span class="sxs-lookup"><span data-stu-id="fb1f4-127">These reports are used to monitor and improve the overall performance of the service.</span></span>
