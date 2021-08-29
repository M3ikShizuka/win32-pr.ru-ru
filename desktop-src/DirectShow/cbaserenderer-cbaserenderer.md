---
description: Метод конструктора Кбасерендерер. Кбасерендерер.
ms.assetid: df5efbb3-6bce-4e30-b1b1-d69bf64fa87d
title: Конструктор Кбасерендерер. Кбасерендерер (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseRenderer.CBaseRenderer
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: b7041444e40aa926efbeebd074d8e8bb736bdd1005c35730dac86a87303927f4
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120044004"
---
# <a name="cbaserenderercbaserenderer-constructor"></a>Кбасерендерер. Кбасерендерер, конструктор

Метод конструктора.

## <a name="syntax"></a>Синтаксис


```C++
CBaseRenderer(
   REFCLSID  RenderClass,
   TCHAR     *pName,
   LPUNKNOWN pUnk,
   HRESULT   *phr,
   UINT      TimerResolution = 1
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*рендеркласс* 
</dt> <dd>

Идентификатор класса модуля подготовки отчетов.

</dd> <dt>

*pName* 
</dt> <dd>

Указатель на строку, содержащую имя фильтра, для целей отладки.

</dd> <dt>

*pUnk* 
</dt> <dd>

Указатель на владельца этого объекта. Если объект является агрегатным, передайте указатель на интерфейс **IUnknown** объекта агрегирования. В противном случае присвойте этому параметру **значение NULL**.

</dd> <dt>

*фр* 
</dt> <dd>

Получает значение **HRESULT** .

</dd> <dt>

*TimerResolution* 
</dt> <dd>

Разрешение таймера.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасерендерер**](cbaserenderer.md)
</dt> </dl>

 

 




