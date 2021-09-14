---
description: Свойство Примарикэйс объекта Database возвращает объект Record, содержащий имя таблицы в поле 0, и имена столбцов (содержащие первичные ключи) в полях, соответствующих их номерам столбцов.
ms.assetid: 9aeafda4-65b8-4469-a391-eb25ca72459d
title: Свойство Database. Примарикэйс
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Database.PrimaryKeys
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: dc266bc2e563e6f32b7ff9b8c7c8cb0df69b723d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127141941"
---
# <a name="databaseprimarykeys-property"></a>Свойство Database. Примарикэйс

Свойство **примарикэйс** объекта [**Database**](database-object.md) возвращает объект [**Record**](record-object.md) , содержащий имя таблицы в поле 0, и имена столбцов (содержащие первичные ключи) в полях, соответствующих их номерам столбцов. Число полей в записи равно числу столбцов первичного ключа.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Database.PrimaryKeys
```



## <a name="property-value"></a>Значение свойства

Обязательное имя существующей таблицы. Если таблица не существует, возникает ошибка.

## <a name="remarks"></a>Remarks

Свойство **примарикэйс** не может использоваться с [ \_ таблицей таблиц](-tables-table.md) или [ \_ столбцами](-columns-table.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ идатабасе определяется как 000C109D-0000-0000-C000-000000000046<br/>                                                                                                                                                                            |



 

 




