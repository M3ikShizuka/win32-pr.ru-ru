---
title: Удаленная служба данных удалена
description: Компоненты сервера удаленной службы данных удаляются в Windows 8
ms.assetid: 53ECB92C-8868-4A1A-82BD-4ADE75F7BB59
keywords:
- Сервер RDS
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 05ee18b62bf78bc30aa07cc861963c03baa90c1fd4bc405207b1586ee6167f58
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119935074"
---
# <a name="remote-data-service-server-components-are-removed-in-windows-8"></a>Компоненты сервера удаленной службы данных удаляются в Windows 8

## <a name="platforms"></a>Платформы

 **клиенты** — Windows 8  
**серверы** — Windows Server 2012  



## <a name="description"></a>Описание

Сервер удаленной службы данных (RDS) недоступен в Windows 8:

-   Файл msadcf.dll, в котором размещается по умолчанию "бизнес-объект" RDSServer. DataObject, удаляется, а связанные с ним файлы (msadcfr.dll, msadcfr.dll. MUI, handler. reg и хандсафе. reg) удаляются.
-   Файл msdfmap.dll, который является обработчиком по умолчанию, удаляется, а файл msdfmap.ini удаляется.
-   Файл msadcs.dll, ISAPI, удален

## <a name="manifestation"></a>Проявление

Клиенты не могут размещать RDS Server на Windows 8.

## <a name="mitigation"></a>Меры по снижению риска

клиенты могут размещать свои RDS-серверы на компьютере с Windows 7 или другими операционными системами нижнего уровня.

## <a name="solution"></a>Решение

клиенты могут размещать свои RDS-серверы на компьютере с Windows 7 или другими операционными системами нижнего уровня.

## <a name="resources"></a>Ресурсы

[Схема технологий доступа к данным](/sql/connect/connect-history?view=sqlallproducts-allversions)

 

 