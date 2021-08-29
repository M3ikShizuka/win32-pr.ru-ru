---
description: Метод конструктора Кдисппарамс. Кдисппарамс.
ms.assetid: da67a5e4-b4a1-4a38-93fe-0965695e93f5
title: Конструктор Кдисппарамс. Кдисппарамс (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CDispParams.CDispParams
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: ba9180358f8398060fe7632c0a75b28f61ffb237638b0d121fccefe7cf3c2f5f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119910024"
---
# <a name="cdispparamscdispparams-constructor"></a>Кдисппарамс. Кдисппарамс, конструктор

Метод конструктора.

## <a name="syntax"></a>Синтаксис


```C++
CDispParams(
   UINT    nArgs,
   VARIANT *pArgs
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*наргс* 
</dt> <dd>

Количество аргументов, переданных методу или свойству.

</dd> <dt>

*паргс* 
</dt> <dd>

Указатель на список аргументов. В списке каждый аргумент сохраняется с типом Variant.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кдисппарамс**](cdispparams.md)
</dt> </dl>

 

 




