---
description: метод OpenView объекта Database возвращает объект представления, представляющий запрос, заданный SQL строкой.
ms.assetid: 6afb2fdb-0e6a-468f-8faf-e48d8d1960b6
title: Метод Database. OpenView (Цертвиев. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Database.OpenView
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 8dc62ca38bfe28980da71ecf63eda8e6c39aaf0a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127141942"
---
# <a name="databaseopenview-method"></a>Database. OpenView, метод

метод **OpenView** объекта [**Database**](database-object.md) возвращает объект [**представления**](view-object.md) , представляющий запрос, заданный SQL строкой.

## <a name="syntax"></a>Синтаксис


```JScript
Database.OpenView(
  sql
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*sql* 
</dt> <dd>

обязательный SQL строки запроса.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

сведения о синтаксисе SQL, реализованном в установщике, см. в разделе [синтаксис SQL](sql-syntax.md).

В случае сбоя метода можно получить расширенные сведения об ошибке с помощью метода [**ластерроррекорд**](installer-lasterrorrecord.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| Заголовок<br/>  | <dl> <dt>Цертвиев. h</dt> </dl>                                                                                                                                                                   |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ идатабасе определяется как 000C109D-0000-0000-C000-000000000046<br/>                                                                                                                                                                            |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**База данных**](database-object.md)
</dt> <dt>

[Синтаксис SQL](sql-syntax.md)
</dt> </dl>

 

 




