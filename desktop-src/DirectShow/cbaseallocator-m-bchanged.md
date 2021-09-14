---
description: Флаг, указывающий, изменились ли требования к буферу.
ms.assetid: 34d946f9-125c-40fb-b09e-82457add07d6
title: 'Элемент Кбасеаллокатор:: m_bChanged (Амфилтер. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- m_bChanged
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 86c700f3c0ee820206613bcf3147652b1826b57a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058126"
---
# <a name="cbaseallocatorm_bchanged-member"></a>Элемент Кбасеаллокатор:: m \_ бчанжед

Флаг, указывающий, изменились ли требования к буферу. Метод [**кбасеаллокатор:: SetProperties**](cbaseallocator-setproperties.md) устанавливает значение **true**. В производном классе чистый виртуальный метод [**кбасеаллокатор:: Alloc**](cbaseallocator-alloc.md) должен вернуть значение **false**. После выделения буферов нет необходимости их повторного выделения, пока *m \_ Бчанжед* имеет **значение false**.

## <a name="syntax"></a>Синтаксис


```C++
BOOL m_bChanged;
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеаллокатор**](cbaseallocator.md)
</dt> </dl>

 

 




