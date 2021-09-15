---
description: Макрос НАПОМНИТЬ о создании напоминания во время компиляции. Этот макрос создает строку, содержащую строку параметра, имя исходного файла и номер строки.
ms.assetid: 12043df5-ed68-4980-91aa-7598d8ab1951
title: НАПОМНИТЬ (Вксдебуг. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- REMIND
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 305e5df628244293b643da8882f57dd83041c4c6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127348922"
---
# <a name="remind"></a>Вам

`REMIND`Макрос создает напоминание во время компиляции. Этот макрос создает строку, содержащую строку параметра, имя исходного файла и номер строки.

``` syntax
REMIND(strLiteral);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="strLiteral"></span><span id="strliteral"></span><span id="STRLITERAL"></span>*стрлитерал*
</dt> <dd>

Текстовая строка.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Этот макрос полезен для создания предупреждений во время компиляции:


```C++
#pragma message (REMIND("TO DO: Add support for IDispatch."))
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксдебуг. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Выходные функции отладки](debug-output-functions.md)
</dt> </dl>

 

 




