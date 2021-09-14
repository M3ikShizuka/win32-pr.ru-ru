---
description: Метод конструктора Кмедиаевент. Кмедиаевент.
ms.assetid: 7f7a0a9f-e531-4e22-8601-b84ab088e9e7
title: Конструктор Кмедиаевент. Кмедиаевент (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CMediaEvent.CMediaEvent
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 36cd82b086241012542701001c4de1fe16ac2d8e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054722"
---
# <a name="cmediaeventcmediaevent-constructor"></a>Кмедиаевент. Кмедиаевент, конструктор

Метод конструктора.

## <a name="syntax"></a>Синтаксис


```C++
CMediaEvent(
   const TCHAR     *pName,
         LPUNKNOWN pUnk
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pName* 
</dt> <dd>

Указатель на имя объекта для целей отладки.

</dd> <dt>

*pUnk* 
</dt> <dd>

Указатель на владельца этого объекта.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Выделите параметр *pName* в статической памяти. Это имя отображается в терминале отладки при создании и удалении объекта.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кмедиаевент**](cmediaevent.md)
</dt> </dl>

 

 




