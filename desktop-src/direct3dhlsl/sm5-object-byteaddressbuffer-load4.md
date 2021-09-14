---
title: 'Функция Битеаддрессбуффер:: Load4 (UINT)'
description: 'Возвращает четыре значения. | Функция Битеаддрессбуффер:: Load4 (UINT)'
ms.assetid: bc74bf29-1c22-4e47-bafc-ecef194f54b8
keywords:
- Функция Load4 HLSL
topic_type:
- apiref
api_name:
- Load4
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 18ce27e7d02a414165aab169e40a6ab14cdd8c4c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055941"
---
# <a name="byteaddressbufferload4uint-function"></a>Функция Битеаддрессбуффер:: Load4 (UINT)

Возвращает четыре значения.

## <a name="syntax"></a>Синтаксис

``` syntax
uint4 Load4(
  in uint address
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*адрес* \[ окне\]
</dt> <dd>

Тип: **uint**

Входной адрес в байтах, который должен быть кратным 4.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **uint4**

Четыре значения.

## <a name="remarks"></a>Комментарии

Эта функция поддерживается для следующих типов шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
| x      | x    | x      | x        | x     | x       |



 

## <a name="see-also"></a>См. также:

<dl> <dt>

[Методы Load4](byteaddressbuffer-load4.md)
</dt> <dt>

[Модель шейдера 5](d3d11-graphics-reference-sm5.md)
</dt> </dl>

 

 




