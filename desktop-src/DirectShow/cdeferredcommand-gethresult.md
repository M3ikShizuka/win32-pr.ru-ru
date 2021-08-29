---
description: Методического HResult извлекает значение HRESULT из вызванной команды.
ms.assetid: 7e88a2bd-6b1b-4e59-b185-5dfd501fc37a
title: Кдеферредкомманд. метод HResult (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CDeferredCommand.GetHResult
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 16513cd202d8ad1973a6aa4d2bfd69f8372cb9b611e1dc070e265685db2d2682
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119910104"
---
# <a name="cdeferredcommandgethresult-method"></a>Кдеферредкомманд. метод HResult

`GetHResult`Метод получает значение **HRESULT** из вызванной команды.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetHResult(
   HRESULT *phrResult
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*фрресулт* 
</dt> <dd>

Указатель на значение **HRESULT** .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает "E \_ Abort", если **m \_ Пкуеуе** имеет **значение NULL**. В противном случае возвращается значение S \_ ОК.

## <a name="remarks"></a>Remarks

Эта функция члена реализует метод [**идеферредкомманд:: и HRESULT**](/windows/desktop/api/Control/nf-control-ideferredcommand-gethresult) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кдеферредкомманд**](cdeferredcommand.md)
</dt> </dl>

 

 




