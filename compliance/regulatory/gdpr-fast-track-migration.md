---
title: GDPR
description: 'Технические рекомендации Майкрософт: НАБОР ИНСТРУМЕНТОВ МИГРАЦИИ С ПОМОЩЬЮ FASTTRACK ДЛЯ ОТПРАВКИ ЗАПРОСОВ НА УДАЛЕНИЕ'
keywords: Миграция с помощью FastTrack, Microsoft 365 для образования, документация по Microsoft 365, GDPR
localization_priority: Priority
Robots: NOFOLLOW,NOINDEX
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: mohitku
author: MohitKumar
manager: laurawi
audience: itpro
ms.collection:
- GDPR
- M365-security-compliance
- MS-Compliance
titleSuffix: Microsoft GDPR
hideEdit: true
ms.openlocfilehash: d3429d3fb35317146e32fddc71bae2f12c40269d
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53089512"
---
# <a name="fasttrack-migration-toolset-for-submitting-delete-request"></a>Набор инструментов миграции с помощью FastTrack для отправки запросов на удаление

## <a name="toolset-purpose"></a>Назначение набора инструментов

Если вы клиент, участвующий в миграции с помощью FastTrack, удаление учетной записи пользователя не приведет к удалению копии данных, хранящейся у специалистов Microsoft FastTrack. Эти данные хранятся исключительно для целей завершения миграции. Если в процессе миграции вам потребуется, чтобы специалисты Microsoft FastTrack удалили имеющуюся у них копию данных, отправьте соответствующий запрос с помощью этого набора инструментов. В обычных обстоятельствах Microsoft FastTrack удаляет все копии данных по завершении миграции организации.

### <a name="supported-platforms"></a>Поддерживаемые платформы

Корпорация Майкрософт поддерживает первоначальный выпуск этого набора инструментов для платформы Windows и консоли PowerShell. Кроме того, этот набор инструментов поддерживает указанные ниже известные платформы.

***Таблица 1. Платформы, поддерживаемые набором инструментов** _

_***

|Версия PowerShell|Windows 7|Windows 8|Windows 10|Windows Server 2012|Windows Server 2016|
|:---:|:---:|:---:|:---:|:---:|:---:|
|5.0|Не поддерживается|Поддерживается|Поддерживается|Поддерживается|Поддерживается|
|5.1|Не поддерживается|Поддерживается|Поддерживается|Поддерживается|Поддерживается|
|

### <a name="obtaining-the-toolset"></a>Получение набора инструментов

Этот набор инструментов доступен в коллекции PowerShell в консольном приложении PowerShell. Чтобы найти и загрузить этот модуль командлета, сначала откройте PowerShell в режиме администратора, чтобы получить соответствующие разрешения для установки модуля. Если ранее вы не использовали PowerShell, в поле поиска на панели задач Windows введите PowerShell. Чтобы запустить Windows PowerShell, щелкните консольное приложение правой кнопкой мыши, выберите **Запуск от имени администратора** и нажмите кнопку **Да**.

![PowerShell: запуск от имени администратора](../media/fasttrack-powershell_image.png)

![PowerShell: предоставление разрешения на внесение изменений приложению](../media/fasttrack-run-powershell_image.png)

Теперь, когда вы открыли консоль, вам потребуется настроить разрешения для выполнения скрипта. Чтобы разрешить выполнение скрипта, введите следующую команду:

```powershell
Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
```

Вам будет предложено подтвердить это действие, так как администратор может изменять область по своему усмотрению.

**_Настройка политики выполнения_* _

![Изменение политики выполнения в PowerShell](../media/powershell-set-execution-policy_image.png)

Теперь, когда для консоли настроено разрешение на выполнение скрипта, установите необходимый модуль, выполнив следующую команду:

```powershell
Install-Module -Name Microsoft.FastTrack -Repository PSGallery -WarningAction SilentlyContinue -Force
```

### <a name="prerequisites-for-module"></a>Компоненты, необходимые для работы модуля

Для успешной работы этого модуля вам может потребоваться установить зависимые модули (если они еще не установлены). Возможно, вам придется перезапустить PowerShell.

Чтобы отправить запрос субъекта данных, вам сначала потребуется выполнить вход, используя свои учетные данные Office 365. Введя соответствующие учетные данные, вы подтвердите свой статус глобального администратора и сможете собирать информацию о клиенте.

```powershell
Login-FastTrackAccount -ApiKey <API Key provided by FastTrack MVM>
```

После успешного входа в систему учетные данные и ключ будут сохранены для использования с модулями FastTrack до конца текущего сеанса PowerShell.

Если вам необходимо подключиться к облачной среде, отличной от коммерческой, нужно добавить к команде *Log in* параметр -Environment* с указанием одной из допустимых сред:

- AzureCloud
- AzureChinaCloud
- AzureGermanCloud
- AzureUSGovernmentCloud

```powershell
Login-FastTrackAccount -ApiKey <API Key provided by FastTrack MVM> -Environment <cloud environment>
```

Чтобы отправить запрос DSR, выполните следующую команду:

```powershell
Submit-FastTrackGdprDsrRequest -DsrRequestUserEmail SubjectUserEmail@mycompany.com
```

При успешном выполнении командлета он возвратит объект идентификатора транзакции. Сохраните этот идентификатор транзакции.

#### <a name="checking-the-status-of-a-request-transaction"></a>Проверка состояния транзакции запроса

Запустите следующую функцию, используя ранее полученный идентификатор транзакции:

```powershell
Get-FastTrackGdprDsrRequest -TransactionID "YourTransactionID"
```

#### <a name="transaction-status-codes"></a>Коды состояния транзакции

|Транзакция|Статус|
|---|---|
|**Создано**|Запрос создан.|
|**Не удалось выполнить**|Не удалось создать запрос. Отправьте запрос еще раз или обратитесь в службу поддержки.|
|**Выполнено**|Запрос был выполнен и очищен.|
|

<!-- original version: **Created**  Request has been created<br/>**Failed** Request failed to create, please resubmit, or contact support<br/>**Completed** Request has been completed and sanitized -->

## <a name="learn-more"></a>Подробнее

[Центр управления безопасностью (Майкрософт)](https://www.microsoft.com/trust-center/privacy/gdpr-overview)
