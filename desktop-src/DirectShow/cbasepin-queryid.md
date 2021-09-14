---
description: 'Метод QueryId извлекает идентификатор ПИН-кода. Этот метод реализует метод Ипин:: QueryId.'
ms.assetid: b365a574-61b4-454c-b062-8826cbe10f03
title: Кбасепин. QueryId, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBasePin.QueryId
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: fa14fb933c89da0b0b6d2eebfab480b5508a3666
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127254485"
---
# <a name="cbasepinqueryid-method"></a>Кбасепин. QueryId, метод

`QueryId`Метод получает идентификатор ПИН-кода. Этот метод реализует метод [**Ипин:: QueryId**](/windows/desktop/api/Strmif/nf-strmif-ipin-queryid) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT QueryId(
   LPWSTR *Id
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Id* 
</dt> <dd>

Указатель на идентификатор ПИН-кода.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** . Возможные значения перечислены в следующей таблице.



| Код возврата                                                                                   | Описание                           |
|-----------------------------------------------------------------------------------------------|---------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>          | Успешно.<br/>                   |
| <dl> <dt>**E \_ OUTOFMEMORY**</dt> </dl> | Недостаточно памяти.<br/>       |
| <dl> <dt>**\_указатель E**</dt> </dl>     | **Пустой** аргумент указателя.<br/> |



 

## <a name="remarks"></a>Remarks

Этот метод возвращает копию переменной-члена [**кбасепин:: m \_ pName**](cbasepin-m-pname.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасепин**](cbasepin.md)
</dt> </dl>

 

 




