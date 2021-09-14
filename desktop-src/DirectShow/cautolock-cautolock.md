---
description: Метод конструктора. Конструктор блокирует указанный объект критической секции.
ms.assetid: 5a0d74f9-bb99-4922-9a92-2e7c1863421f
title: Конструктор Каутолокк. Каутолокк (Вксутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CAutoLock.CAutoLock
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: fed29011d4fe581ed146f64800351a3f1053d957
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127347122"
---
# <a name="cautolockcautolock-constructor"></a>Каутолокк. Каутолокк, конструктор

Метод конструктора. Конструктор блокирует указанный объект критической секции.

## <a name="syntax"></a>Синтаксис


```C++
CAutoLock(
   CCritSec *plock
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*плокк* 
</dt> <dd>

Указатель на объект [**ккритсек**](ccritsec.md) , который содержит объект критической секции.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксутил. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Каутолокк**](cautolock.md)
</dt> </dl>

 

 




