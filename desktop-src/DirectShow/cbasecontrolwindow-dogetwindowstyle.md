---
description: Метод Дожетвиндовстиле извлекает текущие стандартные или расширенные стили окна.
ms.assetid: 1a854896-4bcb-49d0-92e4-40d1923712f9
title: Кбасеконтролвиндов. Дожетвиндовстиле, метод (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseControlWindow.DoGetWindowStyle
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: d970ee52203c5c8dfe8a897c5612604becc2b2e1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126972002"
---
# <a name="cbasecontrolwindowdogetwindowstyle-method"></a>Кбасеконтролвиндов. Дожетвиндовстиле, метод

`DoGetWindowStyle`Метод извлекает текущие стандартные или расширенные стили окна.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT DoGetWindowStyle(
   long *pStyle,
   long WindowLong
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пстиле* 
</dt> <dd>

Указатель на переменную, которая получает сведения о стиле.

</dd> <dt>

*виндовлонг* 
</dt> <dd>

Значение, указывающее, какие стили следует извлечь. Должна быть одной из следующих:



| Метка | Значение |
|--------------|--------------------------------------|
| \_стиль ГВЛ   | Получение стилей окна.          |
| ГВЛ \_ операторе EXSTYLE | Получение расширенных стилей окна. |



 

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Комментарии

Эта функция члена вызывает функцию Win32 **жетвиндовлонг** для получения стиля окна. Он вызывается функциями-членами [**кбасеконтролвиндов:: Get \_ WindowStyle**](cbasecontrolwindow-get-windowstyle.md) и [**кбасеконтролвиндов:: Get \_ виндовстиликс**](cbasecontrolwindow-get-windowstyleex.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеконтролвиндов**](cbasecontrolwindow.md)
</dt> </dl>

 

 




