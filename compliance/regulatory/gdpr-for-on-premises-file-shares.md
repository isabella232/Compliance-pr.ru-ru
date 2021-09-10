---
title: GDPR для локальных общих папок
description: Узнайте, как обеспечить соблюдение требований Общего регламента по защите данных (GDPR) в локальных общих папках Windows Server.
f1.keywords:
- NOCSH
ms.author: mikeplum
author: MikePlumleyMSFT
manager: pamgreen
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: high
titleSuffix: Microsoft GDPR
ms.custom: seo-marvel-apr2020
ms.collection: MS-Compliance
hideEdit: true
ms.openlocfilehash: 9c281b6096512f65f20286948addc32127278b98
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2021
ms.locfileid: "58948491"
---
# <a name="gdpr-for-on-premises-windows-server-file-shares"></a>GDPR для локальных общих папок Windows Server

Основной рекомендуемый подход для общих папок:

-   Используйте Azure Information Protection для пометки конфиденциальных данных.

-   Используйте сканер Azure Information Protection для поиска данных.

Рекомендуемый подход для общих папок включает следующие действия:

1.  **Установите и настройте сканер Azure Information Protection.**

    -   Выберите необходимые типы конфиденциальных данных.

    -   Укажите необходимые локальные и сетевые папки.

2.  **Выполните цикл обнаружения.**

    -   Запустите сканер в режиме обнаружения и проверьте обнаруженные данные.

    -   При необходимости оптимизируйте условия и типы конфиденциальной информации.

    -   Оцените ожидаемое воздействие автоматического применения меток.

3.  **Запустите сканер Azure Information Protection для применения меток к соответствующим документам**.

4.  **Для защиты:**

    -   Настройте правила защиты от потери данных в Exchange, чтобы защитить документы с нужной меткой.

    -   Обязательно используйте разрешения, чтобы ограничить доступ к файлам.

5.  **Интегрируйте журналы Windows Server со средством SIEM для мониторинга.**

    -   Чтобы находить персональные данные для запросов субъектов данных, используйте сканер Azure Information Protection. Вы также можете включить обход общих папок в настройках поиска SharePoint Server.

Дополнительные сведения об использовании сканера Azure Information Protection для поиска и пометки персональных данных см. в разделе [Развертывание сканера AIP](/azure/information-protection/deploy-aip-scanner).

Сведения о настройке сканера в соответствии с условиями и использовании типов конфиденциальной информации для защиты от потери данных (DLP) в Office 365 см. в статье [Как настроить условия для автоматической и рекомендуемой классификации с помощью Azure Information Protection](/information-protection/deploy-use/configure-policy-classification). Обратите внимание, что новые типы конфиденциальной информации Office 365 не сразу станут доступны для использования в сканере. Кроме того, в нем невозможно использовать пользовательские типы конфиденциальной информации.
