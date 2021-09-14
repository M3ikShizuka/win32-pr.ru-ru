---
description: Метод размещения \_ WindowState задает состояние окна.
ms.assetid: 0d22fa84-17bc-4228-b86e-d31857156802
title: Метод CBaseControlWindow.put_WindowState (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseControlWindow.put_WindowState
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 1944e9bd39816cd1f022296b69fdac60d0779f1a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173856"
---
# <a name="cbasecontrolwindowput_windowstate-method"></a>Кбасеконтролвиндов. размещение \_ метода WindowState

`put_WindowState`Метод задает состояние окна.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_WindowState(
   long WindowState
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*WindowState* 
</dt> <dd>

Новое состояние окна.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Remarks

Эта функция-член принимает те же параметры, что и функция Microsoft Win32 **ShowWindow** (например, WS \_ шовнормал, WS \_ шовминноактивате и WS \_ шовмаксимизед).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеконтролвиндов**](cbasecontrolwindow.md)
</dt> </dl>

 

 




