---
description: Сохраняет данные фильтра в заданном потоке.
ms.assetid: f45c8c6e-f0bb-4358-805a-da2669706d34
title: Метод Кперсистстреам. Save (Пстреам. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CPersistStream.Save
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 66822a789872ef166d5c5476c496a2543d7896bbba65eddeecf0556ce64ba89f
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119915574"
---
# <a name="cpersiststreamsave-method"></a>Кперсистстреам. Save, метод

Сохраняет данные фильтра в заданном потоке.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Save(
   LPSTREAM pStm,
   BOOL     fClearDirty
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пстм* 
</dt> <dd>

Указатель на поток, в который должны быть сохранены данные.

</dd> <dt>

*фклеардирти* 
</dt> <dd>

Флаг, указывающий, следует ли сбрасывать флаг "грязный" текущего потока; **Значение true** означает сброс. (Если метод вызывается как часть операции сохранения, значение обычно равно **true**; при вызове как часть операции сохранения как значение обычно равно **false**.)

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Remarks

Эта функция члена реализует метод **IPersistStream:: Save** . Он вызывает **вритеинт** с версией программного обеспечения, [**вызывает Кперсистстреам:: вритетостреам**](cpersiststream-writetostream.md) с потоком в *пстм* и сбрасывает **mPS \_ фдирти**.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>пстреам. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кперсистстреам**](cpersiststream.md)
</dt> </dl>

 

 




