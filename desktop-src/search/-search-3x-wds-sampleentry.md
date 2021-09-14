---
description: в этом разделе описываются технологии, связанные с Windowsным поиском.
ms.assetid: 76b39ea6-2aaf-40e0-aa56-2165e188244d
title: Связанные технологии поиска
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 704f8a03738958e19712ff8cc4566e4b7f7396ca
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127262579"
---
# <a name="related-search-technologies"></a>Связанные технологии поиска

в этом разделе описываются технологии, связанные с [Windowsным поиском](-search-3x-wds-overview.md).

Этот раздел организован следующим образом:

-   [Enterprise Осуществлять](#enterprise-search)
    -   [SharePoint поиск Enterprise](#sharepoint-enterprise-search)
-   [Windows Поиск на рабочем столе 2. x](#windows-desktop-search-2x)
-   [Пакет Platform SDK: служба индексирования](#platform-sdk-indexing-service)
-   [Связанные темы](#related-topics)

## <a name="enterprise-search"></a>Enterprise Осуществлять

обзор технических ресурсов для [Enterprise поиска в майкрософт](https://www.microsoft.com/enterprisesearch/en/us/default.aspx)см. в следующих статьях:

-   [Enterprise Поиск в центре ресурсов](https://developer.microsoft.com/office/docs)
-   [блог Microsoft Enterprise Search](https://blogs.msdn.com/b/enterprisesearch/rss.aspx)

### <a name="sharepoint-enterprise-search"></a>SharePoint поиск Enterprise

SharePoint Foundation 2010 предоставляет [запросы из кода на стороне сервера](/previous-versions/office/developer/sharepoint-2010/ee536691(v=office.14)) и [запросы из клиентского кода](/previous-versions/office/developer/sharepoint-2010/ee539764(v=office.14)). дополнительные сведения о запросах, поиске нового содержимого и повышении релевантности с помощью Sharepoint Server 2010 Enterprise search см. в разделе [основы поиска Enterprise](/previous-versions/office/ee554857(v=office.14)).

Windows 7 поиск поддерживает службы федерации поиска для удаленных хранилищ данных с помощью OpenSearch технологий, которые позволяют пользователям получать доступ к удаленным данным и взаимодействовать с ними в обозревателе Windows. SharePoint Search Server 2008 и MOSS 2007 с пакетом обновления 2 (SP2) также поддерживают федеративный поиск удаленных серверов с помощью OpenSearch. сведения о развертывании сервера search Server 2008 с Office SharePoint Server 2007 см. в разделе [федеративный поисковый \[ сервер search server 2008 \] ](/previous-versions/office/bb931109(v=office.14)). Сведения об Аспектном поиске в MOSS, в котором результаты поиска перечисляются по категориям, см. в разделе [CodePlex](https://www.codeplex.com/FacetedSearch).

Windows обработчики протоколов поиска используют спецификации проектирования, аналогичные SharePoint Server. они часто взаимозаменяемы. таким образом, если пользователям требуется искать устаревшие базы данных, хранилища электронной почты или другие структуры данных, которые не поддерживаются Windows поиска, необходимо сначала определить, существует ли обработчик протокола для этого хранилища данных, возможно, для использования с другим приложением, например SharePoint Server. В этом случае можно установить обработчик протокола в системе.

## <a name="windows-desktop-search-2x"></a>Windows Поиск на рабочем столе 2. x

использование и разработка версий 2. x Microsoft Windows Desktop Search (WDS) настоятельно не рекомендуется. вместо использования [Windows Desktop search 2. x](../lwef/-search-2x-wds-overview.md)используйте API поиска [Windows](-search-3x-wds-overview.md) и [Windows поиска](-search-reference-entry-page.md).

## <a name="platform-sdk-indexing-service"></a>Пакет Platform SDK: служба индексирования

[Platform SDK: служба индексирования](/previous-versions/windows/desktop/indexsrv/indexsrv-portal) устарела, начиная с Windows XP. вместо этого используйте API [Windows поиска](-search-3x-wds-overview.md) и [Windows поиска](-search-reference-entry-page.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Обзор Windows Search](-search-3x-wds-overview.md)
</dt> <dt>

[Windows Поиск по руководству разработчика](-search-developers-guide-entry-page.md)
</dt> <dt>

[Windows Поиск ссылки](-search-reference-entry-page.md)
</dt> <dt>

[Windows Поиск примеров кода](-search-samples-ovw.md)
</dt> <dt>

[Федеративный поиск в Windows](-search-federated-search-overview.md)
</dt> <dt>

[Windows Глоссарий поиска](search-glossary.md)
</dt> </dl>

 

 
