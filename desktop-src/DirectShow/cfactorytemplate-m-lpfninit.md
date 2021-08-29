---
description: Указатель на функцию, которая вызывается из точки входа библиотеки DLL. Может иметь значение NULL.
ms.assetid: 0769f55b-6f0d-4a89-9d3f-64f211426342
title: 'Элемент Кфакторитемплате:: m_lpfnInit (Комбасе. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- m_lpfnInit
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: c9f4a12c03e7e001845437f57f9799c7b0861f4f8f9b6cfac56aaa2bb80e51a6
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119566924"
---
# <a name="cfactorytemplatem_lpfninit-member"></a>Элемент Кфакторитемплате:: m \_ лпфнинит

Указатель на функцию, которая вызывается из точки входа библиотеки DLL. Может иметь **значение NULL**.

## <a name="syntax"></a>Синтаксис


```C++
LPFNInitRoutine m_lpfnInit;
```



## <a name="remarks"></a>Remarks

Тип указателя функции — [**лпфнинитраутине**](lpfninitroutine.md). При предоставлении этой функции в библиотеке DLL функция точки входа DLL вызывает ее со следующими параметрами:

-   *блоадинг*: **true** при загрузке библиотеки DLL, **значение false** при выгрузке библиотеки DLL.
-   *рклсид*: указатель на clisd инициализированного объекта, указанный в переменной члена [**\_ CLSID кфакторитемплате:: m**](cfactorytemplate-m-clsid.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>комбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кфакторитемплате**](cfactorytemplate.md)
</dt> </dl>

 

 




