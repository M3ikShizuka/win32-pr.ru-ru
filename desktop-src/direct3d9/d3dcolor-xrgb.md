---
description: Инициализирует цвет с переданными значениями красного, зеленого и синего.
ms.assetid: 832a4a78-c166-4e45-a907-57730da1c2c8
title: Макрос D3DCOLOR_XRGB (D3d9types. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DCOLOR_XRGB
api_type:
- HeaderDef
api_location:
- D3d9types.h
ms.openlocfilehash: 4932e34979b0913f27874e57cfa881f18fb16364
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127258512"
---
# <a name="d3dcolor_xrgb-macro"></a>\_Макрос D3DCOLOR ксргб

Инициализирует цвет с переданными значениями красного, зеленого и синего.

## <a name="syntax"></a>Синтаксис


```C++
D3DCOLOR D3DCOLOR_XRGB(
   int r,
   int g,
   int b
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*r* 
</dt> <dd>

Красный компонент цвета. Это значение должно находиться в диапазоне от 0 до 255.

</dd> <dt>

*g* 
</dt> <dd>

Зеленый компонент цвета. Это значение должно находиться в диапазоне от 0 до 255.

</dd> <dt>

*b* 
</dt> <dd>

Синий компонент цвета. Это значение должно находиться в диапазоне от 0 до 255.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение [**D3DCOLOR**](d3dcolor.md) , соответствующее указанным значениям RGB.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3d9types. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Макросы](dx9-graphics-reference-d3d-macros.md)
</dt> <dt>

[**D3DCOLOR \_ ARGB**](d3dcolor-argb.md)
</dt> <dt>

[**D3DCOLOR \_ RGBA**](d3dcolor-rgba.md)
</dt> </dl>

 

 




