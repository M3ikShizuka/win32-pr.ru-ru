---
description: Метод Крендереринпутпин является методом-конструктором.
ms.assetid: 272f864e-d6a8-4a9e-b72f-892147db9970
title: Конструктор Крендереринпутпин. Крендереринпутпин (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CRendererInputPin.CRendererInputPin
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 2b6970b056706e7443cc38793a9c050d4f93c5ebd86556ce58aff23d4e9e83e7
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120079324"
---
# <a name="crendererinputpincrendererinputpin-constructor"></a>Крендереринпутпин. Крендереринпутпин, конструктор

`CRendererInputPin`Метод является методом-конструктором.

## <a name="syntax"></a>Синтаксис


```C++
CRendererInputPin(
   CBaseRenderer *pRenderer,
   HRESULT       *phr,
   LPCWSTR       Name
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*прендерер* 
</dt> <dd>

Указатель на объект [**кбасерендерер**](cbaserenderer.md) , реализующий фильтр.

</dd> <dt>

*фр* 
</dt> <dd>

Указатель на переменную, которая получает значение **HRESULT** .

</dd> <dt>

*Имя* 
</dt> <dd>

Указатель на строку расширенных символов, содержащую идентификатор ПИН-кода.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Крендереринпутпин**](crendererinputpin.md)
</dt> </dl>

 

 




