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
ms.openlocfilehash: 5b09049bc443991dabe07a7626ffc42097feceee
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053559"
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

## <a name="remarks"></a>Комментарии

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

 

 




