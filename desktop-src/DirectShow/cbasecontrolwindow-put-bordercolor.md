---
description: Метод «разместить \_ BorderColor» изменяет цвет границы.
ms.assetid: bb19d338-7fd1-448c-be94-1c71d4a9a330
title: Метод CBaseControlWindow.put_BorderColor (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseControlWindow.put_BorderColor
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: bc696efd1500d7cb2b9d66efcd8a1ccaa2fa215c1dd0c03516313b3766ff5dad
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119635903"
---
# <a name="cbasecontrolwindowput_bordercolor-method"></a>Кбасеконтролвиндов. размещение \_ BorderColor, метод

`put_BorderColor`Метод изменяет цвет границы.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_BorderColor(
   long Color
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Цвет* 
</dt> <dd>

Новый цвет границы.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Remarks

Приложение может установить конечный прямоугольник, в котором должно отображаться видео. Этот прямоугольник отсчитывается относительно клиентской области окна. Если это сделано (по умолчанию всегда закрашивать все окно), то вокруг видео отображается граница. Это свойство влияет на цвет, используемый границей. Хотя параметр указан как тип **Long** , он фактически является значением **COLORREF** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеконтролвиндов**](cbasecontrolwindow.md)
</dt> </dl>

 

 




