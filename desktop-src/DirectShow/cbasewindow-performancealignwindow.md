---
description: Метод Перформанцеалигнвиндов совмещает расположение окна до границ DWORD, что обеспечивает максимальную производительность.
ms.assetid: e28950bc-2510-45b9-9c9c-c2a9dbc3dc02
title: Кбасевиндов. Перформанцеалигнвиндов, метод (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseWindow.PerformanceAlignWindow
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: e6e7a54372743d430cd904f47c79414d149cf033
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971741"
---
# <a name="cbasewindowperformancealignwindow-method"></a>Кбасевиндов. Перформанцеалигнвиндов, метод

`PerformanceAlignWindow`Метод совмещает расположение окна до границ **DWORD** , что обеспечивает максимальную производительность.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT PerformanceAlignWindow();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ ОК.

## <a name="remarks"></a>Комментарии

Этот метод выровняйте левый и верхний края окна до границ DWORD, что может повысить производительность. Если окно имеет родителя, метод возвращает значение S ОК, \_ но выполняет выравнивание.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасевиндов**](cbasewindow.md)
</dt> </dl>

 

 




