---
description: 'Метод Move размещает и изменяет размер диалогового окна. Этот метод реализует метод Ипропертипаже:: Move.'
ms.assetid: b6cabb5c-196d-489b-9dd4-194d26f4de83
title: Метод Кбасепропертипаже. Move (Кпроп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBasePropertyPage.Move
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 274295c08895fe28b0f3abe3438496719f7fcdfa2dae486401de6babb624cc31
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120052554"
---
# <a name="cbasepropertypagemove-method"></a>Кбасепропертипаже. Move, метод

`Move`Метод размещает и изменяет размер диалогового окна. Этот метод реализует метод **ипропертипаже:: Move** .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Move(
   LPCRECT prect
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*прект* 
</dt> <dd>

Указатель на структуру **Rect** , содержащую сведения о размещении.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** . Ниже приведены возможные значения.



| Код возврата                                                                                  | Описание                           |
|----------------------------------------------------------------------------------------------|---------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>         | Успешно.<br/>                   |
| <dl> <dt>**\_указатель E**</dt> </dl>    | **Пустой** аргумент указателя.<br/> |
| <dl> <dt>**\_непредвиденная E**</dt> </dl> | Непредвиденный сбой.<br/>        |



 

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>кпроп. h (включает Потоки. h)</dt> </dl>                                                                                     |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кбасепропертипаже**](cbasepropertypage.md)
</dt> </dl>

 

 




