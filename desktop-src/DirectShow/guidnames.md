---
description: гуиднамес — это глобальный массив в DirectShow библиотеке базовых классов, которая содержит строки, представляющие идентификаторы guid, определенные в uuid. h. Этот массив полезен для создания выходных данных отладки.
ms.assetid: 6d72ad1e-588a-4a82-a1c1-e1e7b49df572
title: Гуиднамес (Вксдебуг. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- GuidNames
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 359294d0cf3ab4e2074db5935cbbd604dcc1b250
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127169963"
---
# <a name="guidnames"></a>гуиднамес

`GuidNames`— это глобальный массив в DirectShow библиотеке базовых классов, которая содержит строки, представляющие идентификаторы guid, определенные в uuid. h. Этот массив полезен для создания выходных данных отладки.

``` syntax
char* GuidNames[guid]
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="guid"></span><span id="GUID"></span>*устройства*
</dt> <dd>

Указывает любое значение GUID, определенное в файле заголовков UUID. h.

</dd> </dl>

## <a name="remarks"></a>Remarks

Используйте этот глобальный массив для вывода констант GUID в виде строк. Например, следующий код выводит строку "MEDIATYPE \_ Video" в консоль:


```C++
puts(GuidNames[MEDIATYPE_Video]);
```



Если идентификатор GUID не совпадает, возвращается строка "неизвестное имя GUID". не все DirectShow идентификаторы guid определены в uuid. h.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксдебуг. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Выходные функции отладки](debug-output-functions.md)
</dt> </dl>

 

 




