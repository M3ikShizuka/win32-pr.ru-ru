---
description: 'Кфакторитемплате:: m_lpfnNew член-указатель на функцию, которая создает экземпляр объекта.'
ms.assetid: 86859bf9-e16a-4494-bf1b-1d8ddbc1c805
title: 'Элемент Кфакторитемплате:: m_lpfnNew (Комбасе. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- m_lpfnNew
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: ee4ec8e1503d3b260e025d154624b2d7c09bb49b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127266579"
---
# <a name="cfactorytemplatem_lpfnnew-member"></a>Элемент Кфакторитемплате:: m \_ лпфннев

Указатель на функцию, которая создает экземпляр объекта.

## <a name="syntax"></a>Синтаксис


```C++
LPFNNewCOMObject m_lpfnNew;
```



## <a name="remarks"></a>Remarks

В библиотеке DLL Объявите статическую функцию, которая возвращает указатель на новый экземпляр объекта. В шаблоне фабрики задайте в качестве значения переменной члена **m \_ лпфннев** адрес этой статической функции.

Тип указателя функции — [**лпфнневкомобжект**](lpfnnewcomobject.md).

В следующем примере показана типичная функция для **m \_ лпфннев**:


```C++
CUnknown * WINAPI CMyComponent::CreateInstance(LPUNKNOWN pUnk, HRESULT *pHr) 
{
    CMyComponent *pNewObject = 
        new CMyComponent(NAME("My Component"), pUnk, pHr );

    if (pNewObject == NULL)  
    {
        *phr = E_OUTOFMEMORY;
    }
    return pNewObject;
}
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>комбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кфакторитемплате**](cfactorytemplate.md)
</dt> </dl>

 

 




