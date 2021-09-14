---
description: Метод Ваитевент ожидает, пока заданное событие не будет сигнальным.
ms.assetid: 64880f46-7b8f-4823-9d50-052e30ecf04b
title: Кдинамикаутпутпин. Ваитевент, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CDynamicOutputPin.WaitEvent
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: b27f3c387c82eaeebc119f967deaca8e7314ccd7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054747"
---
# <a name="cdynamicoutputpinwaitevent-method"></a>Кдинамикаутпутпин. Ваитевент, метод

`WaitEvent`Метод ожидает, пока заданное событие не будет сигнальным.

## <a name="syntax"></a>Синтаксис


```C++
static HRESULT WaitEvent(
   HANDLE hEvent
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*хевент* 
</dt> <dd>

Дескриптор события.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** . Возможные значения включают в себя, показанные в следующей таблице.



| Код возврата                                                                                  | Описание                  |
|----------------------------------------------------------------------------------------------|------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>         | Успешно.<br/>          |
| <dl> <dt>**\_непредвиденная E**</dt> </dl> | Непредвиденная ошибка.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кдинамикаутпутпин**](cdynamicoutputpin.md)
</dt> </dl>

 

 




