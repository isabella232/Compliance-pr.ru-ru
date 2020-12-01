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
ms.openlocfilehash: 5f753b5d522649575f92178e6f9c932d5ae4725f
ms.sourcegitcommit: 626b0076d133e588cd28598c149a7f272fc18bae
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2020
ms.locfileid: "49509004"
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
