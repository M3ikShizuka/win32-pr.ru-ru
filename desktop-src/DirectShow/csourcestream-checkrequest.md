---
description: Метод Чеккрекуест проверяет наличие запроса потока без блокировки.
ms.assetid: b4691dde-abec-4671-bea6-0f22cc4e7c61
title: Метод Ксаурцестреам. Чеккрекуест (Source. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSourceStream.CheckRequest
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 3100d449d2f29b2080541c5968cad6abc5643b26
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065703"
---
# <a name="csourcestreamcheckrequest-method"></a>Ксаурцестреам. Чеккрекуест, метод

`CheckRequest`Метод проверяет наличие запроса потока без блокировки.

## <a name="syntax"></a>Синтаксис


```C++
BOOL CheckRequest(
   Command *pCom
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пком* 
</dt> <dd>

Указатель на переменную, которая получает значение, переданное в последнем вызове метода [**камсреад:: каллворкер**](camthread-callworker.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если имеется ожидающий запрос, или **false** в противном случае.

## <a name="remarks"></a>Remarks

Этот метод переопределяет метод [**камсреад:: чеккрекуест**](camthread-checkrequest.md) для выполнения проверки типа. Класс **ксаурцестреам** определяет следующий перечислимый тип для параметра *пком* :


```C++
enum Command {CMD_INIT, CMD_PAUSE, CMD_RUN, CMD_STOP, CMD_EXIT};
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Source. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ксаурцестреам**](csourcestream.md)
</dt> </dl>

 

 




