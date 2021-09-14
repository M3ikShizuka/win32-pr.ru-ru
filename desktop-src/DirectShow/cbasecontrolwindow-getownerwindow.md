---
description: Метод Жетовнервиндов Извлекает маркер окна-владельца m \_ хвндовнер.
ms.assetid: fa576b42-b4a7-4374-8ba4-7d21e86d9d61
title: Кбасеконтролвиндов. Жетовнервиндов, метод (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseControlWindow.GetOwnerWindow
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 4e4d3811f85abd68bcd7d625dce0e9e8963be39a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971922"
---
# <a name="cbasecontrolwindowgetownerwindow-method"></a>Кбасеконтролвиндов. Жетовнервиндов, метод

`GetOwnerWindow`Метод получает маркер окна-владельца, **m \_ хвндовнер**.

## <a name="syntax"></a>Синтаксис


```C++
HWND GetOwnerWindow();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает окно владельца.

## <a name="remarks"></a>Комментарии

Извлекает окно-владелец без вызова метода интерфейса. Используйте эту функцию-член вместо [**кбасеконтролвиндов:: Get \_ owner**](cbasecontrolwindow-get-owner.md), если только вы не вызываете ее извне с помощью метода [**ивидеовиндов:: Get \_ owner**](/windows/desktop/api/Control/nf-control-ivideowindow-get_owner) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеконтролвиндов**](cbasecontrolwindow.md)
</dt> </dl>

 

 




