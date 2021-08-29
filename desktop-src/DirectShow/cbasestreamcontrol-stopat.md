---
description: 'Метод StopAt информирует ПИН-код, когда следует отказаться от доставки данных. Этот метод реализует метод Иамстреамконтрол:: StopAt.'
ms.assetid: cc9f0fdc-253b-4feb-95ce-56ebc575a49b
title: Метод Кбасестреамконтрол. StopAt (Стрмктл. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseStreamControl.StopAt
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 2cab57715a5b34110e8d92d9829f8b9bc6f819af1b5033198451e412f6e2aa21
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119983384"
---
# <a name="cbasestreamcontrolstopat-method"></a>Кбасестреамконтрол. StopAt, метод

`StopAt`Метод информирует ПИН-код, когда следует отказаться от доставки данных. Этот метод реализует метод [**иамстреамконтрол:: StopAt**](/windows/desktop/api/Strmif/nf-strmif-iamstreamcontrol-stopat) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT StopAt(
   const REFERENCE_TIME *ptStop = NULL,
         BOOL           bSendExtra = FALSE,
         DWORD          dwCookie = 0
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*птстоп* 
</dt> <dd>

Указатель на значение [**\_ времени ссылки**](reference-time.md) , указывающее, когда ПИН-код должен прекращать доставку данных.

</dd> <dt>

*бсендекстра* 
</dt> <dd>

Задает логическое значение, указывающее, следует ли отправить дополнительный пример после запланированного времени окончания. Если **значение — true**, ПИН-код отправляет один дополнительный пример.

</dd> <dt>

*двкукие* 
</dt> <dd>

Указывает значение для отправки вместе с уведомлением о запуске.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ ОК.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>стрмктл. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасестреамконтрол**](cbasestreamcontrol.md)
</dt> </dl>

 

 




