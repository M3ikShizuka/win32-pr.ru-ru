---
description: HKLM \\ программное обеспечение \\ \\ клиента Microsoft MSSQLSERVER \\ .
ms.assetid: d6eb774b-d7ae-4f51-9947-90fb176e9acf
title: SsASnoversion
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5637a77589d211aae6eb51cacd6376d86367175699b7a339f11f19cc2108b80e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120084744"
---
# <a name="connectto"></a>SsASnoversion

**HKLM \\ программное обеспечение \\ \\ клиента Microsoft MSSQLSERVER \\**

## <a name="description"></a>Описание

в подразделе **ssasnoversion** хранятся сведения о соединении для клиентов на основе Windows, подключающихся к экземплярам компонента Microsoft SQL Server database engine. Записи реестра в этом подразделе имеют тип данных REG \_ SZ, а их значения указывают Net-Library, используемые для подключения к экземпляру, а также любые параметры, относящиеся к сети.

сведения о подключении, хранящиеся в этом подразделе, считываются поставщиком OLE DB для SQL Server, драйвером SQL Server ODBC или библиотекой динамической компоновки SQL Server DB-Library (DLL).

## <a name="change-method"></a>Изменение метода

Не следует изменять записи в этом подразделе с помощью редактора реестра. чтобы настроить имя сервера и сведения о соединении, используйте служебную программу клиента SQL Server Network. дополнительные сведения см. в справке программы SQL Server Client Network.

## <a name="notes"></a>Примечания

-   подключ **ssasnoversion** используется поставщиком OLE DB для SQL Server, драйвером SQL Server ODBC и SQL Server DB-Library DLL. Записи в этом подразделе указывают, какие Net-Library вызывают эти компоненты API доступа к данным.
-   Net-Libraries являются компонентами SQL Server, которые защищают компоненты API доступа к данным из подробных сведений об использовании различных методов межпроцессного взаимодействия (IPC) для взаимодействия с экземпляром ядра субд SQL Server.
-   неправильное обновление подраздела **ssasnoversion** может препятствовать успешному подключению приложений к экземпляру компонента ядра субд SQL Server.

 

 



