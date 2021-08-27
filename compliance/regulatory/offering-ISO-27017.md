---
title: ISO/IEC 27017:2015 "Свод правил по управлению информационной безопасностью"
description: В облачных службах Майкрософт реализованы этот свод правил по управлению информационной безопасностью.
keywords: Microsoft 365, соответствие требованиям, предложения
ms.localizationpriority: high
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmazz
manager: laurawi
audience: itpro
ms.collection:
- M365-security-compliance
- MS-Compliance
hideEdit: true
titleSuffix: Microsoft Compliance
ms.openlocfilehash: b17c7629918bdf4386ad24d28c6cb6687728603c
ms.sourcegitcommit: deff41bc5085d0da42c33dd6d1672be0724a067c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "58561357"
---
# <a name="isoiec-270172015-code-of-practice-for-information-security-controls"></a>ISO/IEC 27017:2015 "Свод правил по управлению информационной безопасностью"

## <a name="iso-iec-27017-overview"></a>Общие сведения о ISO-IEC 27017

Свод правил ISO/IEC 27017:2015 предназначен для организаций для использования в качестве справочника при выборе средств контроля информационной безопасностью облачных служб при реализации системы управления информационной безопасностью облачных вычислений на основе стандарта ISO/IEC 27002:2013. Он также может использоваться поставщиками облачных служб в качестве руководства по реализации общепринятых средств контроля защиты.

Этот международный стандарт предоставляет дополнительные инструкции по внедрению для облачной среды, основанные на стандарте ISO/IEC 27002, и содержит дополнительные средства контроля для устранения облачных рисков и угроз информационной безопасности, ссылаясь на пункты 5-18 стандарта ISO/IEC 27002:2013 со сведениями об средствах контроля, инструкциями реализации и прочей информацией. В частности, этот стандарт предоставляет инструкции по 37 средствам контроля из стандарта ISO/IEC 27002, а также содержит семь новых средств контроля, отсутствующих в стандарте ISO/IEC 27002. Эти новые средства контроля предназначены для следующих важных областей:

- Общие роли и обязанности в облачной среде
- Удаление и возврат ресурсов клиента облачной службы при расторжении договора
- Защита и отделение виртуальной среды клиента от сред других клиентов
- Требования к обеспечению безопасности виртуальной машины для соблюдения бизнес-потребностей
- Процедуры для административных операций с облачной средой
- Разрешение клиентам отслеживать важные действия в облачной среде
- Согласование управления безопасностью для виртуальных и физических сетей

## <a name="microsoft-and-isoiec-27017"></a>Майкрософт и ISO/IEC 27017

ISO/IEC 27017 является уникальным стандартом, предоставляющим руководство как поставщикам облачных служб, так и клиентам облачных служб. Он также содержит практические сведения для клиентов облачных служб о том, что следует ожидать от поставщиков облачных служб. Клиенты могут получить прямую выгоду от использования стандарта ISO/IEC 27017, разобравшись с понятием общей ответственности в облаке.

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Затрагиваемые облачные платформы и службы Майкрософт

- [Azure, Azure для государственных организаций и Azure для Германии](https://aka.ms/AzureCompliance)
- Microsoft Cloud App Security
- [Dynamics 365, Dynamics 365 для государственных учреждений и Dynamics 365 — Германия](https://aka.ms/d365-compliance-list)
- Intune
- Microsoft Defender для конечной точки
- Microsoft Graph
- Microsoft Healthcare Bot
- [Компьютеры, управляемые Майкрософт](/microsoft-365/managed-desktop/intro/compliance)
- Office 365, Office 365 для государственных организаций США, Office 365 U.S. Government Defense и Office 365 Germany
- Облачная служба Power Automate (ранее Microsoft Flow) в виде автономной службы или в составе плана либо набора Office 365 или Dynamics 365
- Облачная служба PowerApps в виде автономной службы или в составе плана либо набора Office 365 или Dynamics 365
- Облачная служба Power BI в виде автономной службы или в составе плана либо набора Office 365
- Power BI Embedded
- Windows 365

## <a name="azure-dynamics-365-and-iso-270172015"></a>Azure, Dynamics 365 и ISO 27017:2015

Дополнительные сведения о соответствии требованиям Azure, Dynamics 365 и другим веб-службам см. в разделе [Предложение Azure ISO 27017](/azure/compliance/offerings/offering-iso-27017).

## <a name="office-365-and-iso-270172015"></a>Office 365 и ISO 27017:2015

### <a name="office-365-cloud-environments"></a>Облачные среды Office 365

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Применимость Office 365 и затрагиваемые службы

Чтобы определить применимость изменений к вашим службам и подписке Office 365, воспользуйтесь следующей таблицей.

| **Применимость** | **Затрагиваемые службы** |
|:------------------|:----------------------|
| **Коммерческий сектор** | Access Online, Azure Active Directory, Azure Communications Service, диспетчер соответствия требованиям, защищенное хранилище, Delve, Exchange Online, Exchange Online Protection, Forms, Griffin, Identity Manager, Lockbox (Torus), Microsoft Defender для Office 365, Microsoft Teams, MyAnalytics, надстройка Office 365 Advanced Compliance, клиентский портал Office 365, микрослужбы Office 365 (в том числе Kaizala, ObjectStore, Sway, служба документов PowerPoint Online, служба аннотации запросов, Синхронизация сведений о школе, Siphon, Speech, StaffHub, программа приложений eXtensible), Центр безопасности и соответствия требованиям Office 365, Office Online, Office Pro Plus, инфраструктура служб Office, OneDrive для бизнеса, Планировщик, PowerApps, Power Automate, Power BI, Project Online, шифрование службы с помощью ключа клиента, SharePoint Online, Skype для бизнеса, Stream |
| **GCC** | Azure Active Directory, Azure Communications Service, диспетчер соответствия требованиям, Delve, Exchange Online, Forms, Microsoft Defender для Office 365, Microsoft Teams, MyAnalytics, надстройка Office 365 Advanced Compliance, Центр безопасности и соответствия требованиям Office 365, Office Online, Office Pro Plus, OneDrive для бизнеса, Планировщик, PowerApps, Power Automate, Power BI, SharePoint Online, Skype для бизнеса, Stream |
| **GCC High** | Azure Active Directory, Azure Communications Service, Exchange Online, Forms, Microsoft Defender для Office 365, Microsoft Teams, надстройка Office 365 Advanced Compliance, Центр безопасности и соответствия требованиям Office 365, Office Online, Office Pro Plus, OneDrive для бизнеса, Планировщик, PowerApps, Power Automate, Power BI, SharePoint Online, Skype для бизнеса |
| **DoD** | Azure Active Directory, Azure Communications Service, Exchange Online, Forms, Microsoft Defender для Office 365, Microsoft Teams, надстройка Office 365 Advanced Compliance, Центр безопасности и соответствия требованиям Office 365, Office Online, Office Pro Plus, OneDrive для бизнеса, Планировщик, Power BI, SharePoint Online, Skype для бизнеса |

### <a name="office-365-audits-reports-and-certificates"></a>Аудит, отчеты и сертификаты Office 365

Аудит облачных служб Майкрософт выполняется раз в год на соответствие своду правил ISO/IEC 27017:2015 в рамках процесса сертификации для ISO/IEC 27001:2013.

- [Office 365: отчет об оценке аудита ISO 27001, 27018 и 27017](https://aka.ms/o365isoreport)

### <a name="frequently-asked-questions"></a>Вопросы и ответы

**К кому применим стандарт?**

Этот свод правил содержит средства контроля и инструкции по реализации для поставщиков облачных служб и клиентов облачных служб. Его структура аналогична стандарту ISO/IEC 27002:2013.

**Где можно посмотреть сведения о соответствии требованиям Майкрософт ISO/IEC 27017:2015?**

Вы можете скачать [сертификат ISO/IEC 27017:2015](https://aka.ms/azureiso27017) для Azure, Intune и Power BI.

**Можно ли использовать соответствие стандарту ISO/IEC 27017 для служб Майкрософт в процессе сертификации моей организации?**

Да. Если ваша организации стремится пройти сертификацию для реализаций, развернутых в любых поддерживаемых корпоративных облачных службах Майкрософт, вы можете использовать соответствующие сертификаты Майкрософт при оценке соответствия требованиям. Однако вы несете ответственность за привлечение аудитора для оценки реализации на соответствие требованиям, а также оценки средств управления и процессов в рамках вашей организации.

**Как получить копии соответствующих отчетов об аудите?**

На портале [Service Trust Portal](https://aka.ms/stphelp) доступны отчеты о независимом аудите и другие сопутствующие документы. Вы можете использовать этот портал для скачивания и просмотра этих документов, помогающих выполнять нормативные требования.

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>Оценка риска с помощью диспетчера соответствия требованиям (Майкрософт)

[Диспетчер соответствия требованиям (Майкрософт)](/microsoft-365/compliance/compliance-manager) — это предварительная функция в [Центре соответствия требованиям Microsoft 365](/microsoft-365/compliance/microsoft-365-compliance-center), помогающая понять состояние вашей организации в отношении соответствия требованиям и принять меры по снижению рисков. Диспетчер соответствия требованиям предоставляет премиум-шаблон для оценки этих нормативных требований. Шаблон находится на странице **шаблонов оценки** в диспетчере соответствия требованиям. См. [Создание оценки в диспетчере соответствия требованиям](/microsoft-365/compliance/compliance-manager-assessments).

### <a name="resources"></a>Ресурсы

- [Свод правил ISO/IEC 27017:2015](https://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=43757)
- [Условия использования веб-служб Майкрософт](https://aka.ms/Online-Services-Terms)
- [Соответствие требованиям в центре управления безопасностью Майкрософт](https://www.microsoft.com/trust-center/compliance/compliance-overview)
