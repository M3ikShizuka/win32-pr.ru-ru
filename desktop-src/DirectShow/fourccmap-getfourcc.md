---
description: Извлекает объект FOURCC&\# 160; DWORD из объекта фаурккмап.
ms.assetid: bb382a57-8499-44c0-b287-2d31f5f5d1d0
title: 'Метод Фаурккмап:: Жетфауркк (FourCC. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- FOURCCMap.GetFOURCC
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: c76493ff172f7a5611367fd50aa3b7957cf5441b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053918"
---
# <a name="fourccmapgetfourcc-method"></a>Метод Фаурккмап:: Жетфауркк

Извлекает DWORD **FourCC**  из объекта [**фаурккмап**](fourccmap.md) .

## <a name="syntax"></a>Синтаксис


```C++
DWORD GetFOURCC();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение  **типа DWORD** . Обратите внимание, что при создании **идентификатора GUID** , который изначально не был производным от **FourCC**, возвращаемое значение будет фактически случайным.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Fourcc. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Фаурккмап**](fourccmap.md)
</dt> </dl>

 

 




