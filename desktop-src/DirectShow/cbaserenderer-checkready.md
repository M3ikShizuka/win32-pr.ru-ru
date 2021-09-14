---
description: Метод Чеккреади запрашивает, завершена ли смена состояния.
ms.assetid: dfa669ed-a5ab-498e-9fc2-ff15d6ddbc13
title: Кбасерендерер. Чеккреади, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseRenderer.CheckReady
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 28c0c8bcb6efb0e3cbd648c1e45d36e8b18d4b74
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127147937"
---
# <a name="cbaserenderercheckready-method"></a>Кбасерендерер. Чеккреади, метод

`CheckReady`Метод запрашивает, завершена ли смена состояния.

## <a name="syntax"></a>Синтаксис


```C++
BOOL CheckReady();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если переход состояния завершен, или **false** , если фильтр все еще переходит в новое состояние.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасерендерер**](cbaserenderer.md)
</dt> <dt>

[**Кбасерендерер:: NotReady**](cbaserenderer-notready.md)
</dt> <dt>

[**Кбасерендерер:: Ready**](cbaserenderer-ready.md)
</dt> </dl>

 

 




