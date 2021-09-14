---
description: Критическая секция, защищающая состояние блокировки.
ms.assetid: 6d20cf4c-2c27-41e6-8d01-6cb5e3876a38
title: 'Элемент Кдинамикаутпутпин:: m_BlockStateLock (Амфилтер. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- m_BlockStateLock
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 56d9175342218e8b82698fe9b89d15937d6913e1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053975"
---
# <a name="cdynamicoutputpinm_blockstatelock-member"></a>Элемент Кдинамикаутпутпин:: m \_ блоккстателокк

Критическая секция, защищающая состояние блокировки.

## <a name="syntax"></a>Синтаксис


```C++
CCritSec m_BlockStateLock;
```



## <a name="remarks"></a>Remarks

Перед использованием любой из следующих переменных члена следует сохранить этот критический раздел:

-   [**Кдинамикаутпутпин:: m \_ блоккстате**](cdynamicoutputpin-m-blockstate.md)
-   [**Кдинамикаутпутпин:: m \_ двблокккаллерсреадид**](cdynamicoutputpin-m-dwblockcallerthreadid.md)
-   [**Кдинамикаутпутпин:: m \_ двнумаутстандингаутпутпинусерс**](cdynamicoutputpin-m-dwnumoutstandingoutputpinusers.md)
-   [**Кдинамикаутпутпин:: m \_ хнотификаллерпинблоккедевент**](cdynamicoutputpin-m-hnotifycallerpinblockedevent.md)

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кдинамикаутпутпин**](cdynamicoutputpin.md)
</dt> </dl>

 

 




