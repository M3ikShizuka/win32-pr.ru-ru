---
description: Обработчик для потока.
ms.assetid: 93d1182a-58f0-4570-8568-fe0fded762cb
title: 'Элемент Камсреад:: m_hThread (Вксутил. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- m_hThread
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: e83dd225da0c3673f9c7f423e0bf56da7431b097
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145169"
---
# <a name="camthreadm_hthread-member"></a>Элемент Камсреад:: m \_ хсреад

Обработчик для потока.

## <a name="syntax"></a>Синтаксис


```C++
HANDLE m_hThread;
```



## <a name="remarks"></a>Remarks

Эта переменная инициализируется как **null**. Метод [**камсреад:: Create**](camthread-create.md) присваивает этой переменной значение обработчика потока. Чтобы определить, существует ли поток, вызовите метод [**камсреад:: среадексистс**](camthread-threadexists.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксутил. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Камсреад**](camthread.md)
</dt> </dl>

 

 




