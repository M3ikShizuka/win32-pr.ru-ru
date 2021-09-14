---
description: Функция LoadOLEAut32 загружает библиотеку динамической компоновки (OleAut32.dll).
ms.assetid: af907341-1e2c-4c63-bf4e-d6c49b4f6a6e
title: Функция LoadOLEAut32 (Комбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- LoadOLEAut32
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: b23bad7e445eebc78ecf8a849ddde8fc23746131
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055446"
---
# <a name="loadoleaut32-function"></a>Функция LoadOLEAut32

Функция **LoadOLEAut32** загружает библиотеку динамической компоновки (OleAut32.dll).

## <a name="syntax"></a>Синтаксис


```C++
HINSTANCE LoadOLEAut32(void);
```



## <a name="parameters"></a>Параметры

У этой функции нет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает маркер для экземпляра библиотеки DLL службы автоматизации.

## <a name="remarks"></a>Комментарии

Когда деструктор [**кбасеобжект**](cbaseobject.md) уничтожает объект, который загрузил OleAut32.dll, он выгружает библиотеку, если она все еще загружена.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>комбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**Вспомогательные функции COM**](com-helper-functions.md)
</dt> </dl>

 

 




