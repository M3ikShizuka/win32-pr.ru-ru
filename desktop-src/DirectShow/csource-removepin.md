---
description: Метод Ремовепин удаляет указанный ПИН-код из фильтра. Метод не удаляет ПИН-код.
ms.assetid: 104eccfa-3fff-4f47-ba1b-3206eab9eef8
title: Метод Ксаурце. Ремовепин (Source. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSource.RemovePin
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: b71ced14a6f92a3056ac4f42e55bc3858c578ff6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057984"
---
# <a name="csourceremovepin-method"></a>Ксаурце. Ремовепин, метод

`RemovePin`Метод удаляет указанный ПИН-код из фильтра. Метод не удаляет ПИН-код.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT RemovePin(
   CSourceStream *pStream
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пстреам* 
</dt> <dd>

Указатель на объект [**ксаурцестреам**](csourcestream.md) , который реализует ПИН-код.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из значений **HRESULT** , приведенных в следующей таблице.



| Код возврата                                                                             | Описание                                      |
|-----------------------------------------------------------------------------------------|--------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>    | Успешно.<br/>                              |
| <dl> <dt>**S \_ false**</dt> </dl> | Фильтр не содержит этот ПИН-код.<br/> |



 

## <a name="remarks"></a>Remarks

Метод деструктора вызывает этот метод, чтобы удалить закрепление вывода из фильтра.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Source. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ксаурце**](csource.md)
</dt> </dl>

 

 




