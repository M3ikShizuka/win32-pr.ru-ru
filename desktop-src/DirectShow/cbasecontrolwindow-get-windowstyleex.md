---
description: Метод Get \_ виндовстиликс извлекает расширенные стили окна.
ms.assetid: 72955958-bbda-4b8f-9c28-6d3f5eb56a82
title: Метод CBaseControlWindow.get_WindowStyleEx (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseControlWindow.get_WindowStyleEx
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: c59336ab57e92e99366494a272f2b995191b494b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971933"
---
# <a name="cbasecontrolwindowget_windowstyleex-method"></a>Кбасеконтролвиндов. Get \_ виндовстиликс, метод

`get_WindowStyleEx`Метод получает расширенные стили окна.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_WindowStyleEx(
   long *pWindowStyleEx
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пвиндовстиликс* 
</dt> <dd>

Указатель на расширенные стили окна.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Комментарии

Эта функция члена получает расширенные стили окна. Он вызывает функцию члена [**кбасеконтролвиндов::D ожетвиндовстиле**](cbasecontrolwindow-dogetwindowstyle.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеконтролвиндов**](cbasecontrolwindow.md)
</dt> </dl>

 

 




