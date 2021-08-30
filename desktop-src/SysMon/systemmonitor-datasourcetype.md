---
title: Системмонитор DataSourceType, свойство
description: Возвращает или задает источник данных счетчика производительности.
ms.assetid: 53c1e9bc-dafd-445c-8d82-13a74f6c488a
keywords:
- Сисмон свойство DataSourceType
- Свойство DataSourceType Сисмон, интерфейс Системмонитор
- Интерфейс Системмонитор Сисмон, свойство DataSourceType
topic_type:
- apiref
api_name:
- SystemMonitor.DataSourceType
api_location:
- Sysmon.ocx
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 79adffc396a581daee16218fc5d39a6480805f0f
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122481860"
---
# <a name="systemmonitordatasourcetype-property"></a>Системмонитор: свойство Атасаурцетипе:D

Возвращает или задает источник данных счетчика производительности.

## <a name="syntax"></a>Синтаксис


```VB
Property DataSourceType As DataSourceTypeConstants
```



## <a name="property-value"></a>Значение свойства

Источник данных счетчика производительности. Возможные значения см. в разделе [**датасаурцетипеконстантс**](/windows/win32/api/isysmon/ne-isysmon-datasourcetypeconstants).

## <a name="exceptions"></a>Исключения




| Тип исключения | Условие | 
|----------------|-----------|
| <strong>System.ArgumentException</strong> | Это исключение может быть получено по одной из следующих причин:<ul><li>Указано недопустимое значение источника данных.</li><li>Если источником данных является файл журнала, СИСМОН не может найти один из указанных файлов. Значение Err. Number — 0xC0000BD1.</li></ul> | 




 

## <a name="remarks"></a>Комментарии

**до Windows Vista:** Невозможно добавить или удалить файлы журнала из [**коллекции файлов журнала**](systemmonitor-logfiles.md) , если для этого свойства задано значение сисмонлогфилес. Присвойте этому свойству значение Сисмонлогфилес после создания или изменения коллекции файлов журнала.

Кроме того, нельзя изменить свойства [**склдсннаме**](systemmonitor-sqldsnname.md) и [**скллогсетнаме**](systemmonitor-sqllogsetname.md) , если для этого свойства не должно быть задано значение сисмонскллог. Присвойте этому свойству значение Сисмонскллог после изменения имен сервера и базы данных.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                            |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                  |
| DLL<br/>                      | <dl> <dt>Сисмон. ocx</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**системмонитор**](systemmonitor.md)
</dt> </dl>

 

 





