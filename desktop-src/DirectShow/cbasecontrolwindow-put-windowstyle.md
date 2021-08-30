---
description: Метод размещения \_ WindowStyle задает стандартные стили окна.
ms.assetid: 3b3aa035-6aa1-4f11-80d8-03268fcf98e1
title: Метод CBaseControlWindow.put_WindowStyle (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseControlWindow.put_WindowStyle
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 416f222b3b4a3f3d10c12baf482d1c94687ba23596fcfbc92e59e1b7dab731e2
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120056732"
---
# <a name="cbasecontrolwindowput_windowstyle-method"></a>Кбасеконтролвиндов. размещение \_ метода WindowStyle

`put_WindowStyle`Метод задает стандартные стили окна.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_WindowStyle(
   long WindowStyle
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*WindowStyle* 
</dt> <dd>

Новые стили окна.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

Следите за изменениями стилей окна. В большинстве случаев приложение должно получить текущий стиль, а затем добавить или удалить недопустимые биты. эта процедура позволяет не менять различные внутренние стили окна, используемые Windows.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кбасеконтролвиндов**](cbasecontrolwindow.md)
</dt> </dl>

 

 




