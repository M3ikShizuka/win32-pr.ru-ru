---
title: 'Рвструктуредбуффер: функция Екременткаунтер:D (Хттпсерв. h)'
description: Уменьшает значение скрытого счетчика объекта.
ms.assetid: 24bc0b63-a482-4fa5-9898-2d43bca20cf4
keywords:
- Функция Декременткаунтер HLSL
topic_type:
- apiref
api_name:
- DecrementCounter
api_location:
- httpserv.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a56641054bb4e9ed4b1865d00c662b0de2afa1a0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127174712"
---
# <a name="decrementcounter-function"></a>Функция Декременткаунтер

Уменьшает значение скрытого счетчика объекта.

## <a name="syntax"></a>Синтаксис

``` syntax
uint DecrementCounter(void);
```

## <a name="parameters"></a>Параметры

У этой функции нет параметров.

## <a name="return-value"></a>Возвращаемое значение

Тип: **uint**

Значение счетчика после уменьшения.

## <a name="remarks"></a>Remarks

Для связанного представления неупорядоченного доступа должен быть [**установлен \_ \_ \_ \_ Счетчик флагов UAV buffer D3D11**](/windows/desktop/api/d3d11/ne-d3d11-d3d11_buffer_uav_flag) во время работы креатионфор этого метода.

Эта функция поддерживается для следующих типов шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
|        |      |        |          | x     | x       |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Хттпсерв. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[рвструктуредбуффер](sm5-object-rwstructuredbuffer.md)
</dt> <dt>

[Модель шейдера 5](d3d11-graphics-reference-sm5.md)
</dt> </dl>

 

