---
title: GDPR для Project Server
description: Узнайте, как обеспечить соблюдение требований общего регламента по защите данных (GDPR) в локальном развертывании Project Server.
f1.keywords:
- NOCSH
ms.author: mikeplum
author: MikePlumleyMSFT
manager: pamgreen
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: Priority
titleSuffix: Microsoft GDPR
ms.custom: seo-marvel-apr2020
ms.collection: MS-Compliance
hideEdit: true
ms.openlocfilehash: ddbf22523caf1869d0253599216fff07ee14f751
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51495953"
---
# <a name="gdpr-for-project-server"></a>GDPR для Project Server

Project Server использует специальные скрипты для экспорта и редактирования данных пользователя в Project Web App. Ниже описывается базовый процесс.

1.  Найдите сайты Project Web App в ферме.

2.  Найдите на каждом сайте проекты, содержащие данные пользователя.

3.  Экспортируйте и просмотрите нужные типы данных.

4.  Отредактируйте данные надлежащим образом.

Эти действия подробно рассматриваются в следующих статьях:

- [Экспорт данных пользователя из Project Server](/Project/export-user-data-from-project-server?toc=/Office365/Enterprise/toc.json)

- [Удаление данных пользователя из Project Server](/Project/delete-user-data-from-project-server?toc=/Office365/Enterprise/toc.json)


Обратите внимание, что Project Server основан на SharePoint Server и регистрирует события в журналах ULS SharePoint и базе данных использования. Дополнительные сведения см. в статье [GDPR для SharePoint Server](gdpr-for-sharepoint-server.md).
