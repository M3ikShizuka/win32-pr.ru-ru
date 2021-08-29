---
description: Определяет константы, описывающие форматы буферов глубины.
ms.assetid: 5e5ce48b-8859-43e0-a9b4-5972cf6bf781
title: Перечисление D3DZBUFFERTYPE (D3D9Types. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DZBUFFERTYPE
api_type:
- HeaderDef
api_location:
- D3D9Types.h
ms.openlocfilehash: f9a04cbc9281009ee0b270cc2dfd7b73e23a5378a2116362f63344c8d7475d7b
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119986344"
---
# <a name="d3dzbuffertype-enumeration"></a>Перечисление D3DZBUFFERTYPE

Определяет константы, описывающие форматы буферов глубины.

## <a name="syntax"></a>Синтаксис


```C++
typedef enum D3DZBUFFERTYPE { 
  D3DZB_FALSE        = 0,
  D3DZB_TRUE         = 1,
  D3DZB_USEW         = 2,
  D3DZB_FORCE_DWORD  = 0x7fffffff
} D3DZBUFFERTYPE, *LPD3DZBUFFERTYPE;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="D3DZB_FALSE"></span><span id="d3dzb_false"></span>**D3DZB \_ false**
</dt> <dd>

Отключить буферизацию глубины.

</dd> <dt>

<span id="D3DZB_TRUE"></span><span id="d3dzb_true"></span>**D3DZB \_ true**
</dt> <dd>

Включить z-буферизацию.

</dd> <dt>

<span id="D3DZB_USEW"></span><span id="d3dzb_usew"></span>**D3DZB \_ усев**
</dt> <dd>

Включить w-Buffering.

</dd> <dt>

<span id="D3DZB_FORCE_DWORD"></span><span id="d3dzb_force_dword"></span>**D3DZB \_ Force \_ DWORD**
</dt> <dd>

Заставляет это перечисление компилироваться до 32 бит в размере. Без этого значения некоторые компиляторы позволяли бы компилировать это перечисление до размера, отличного от 32 бит. Это значение не используется.

</dd> </dl>

## <a name="remarks"></a>Remarks

Члены этого перечислимого типа используются с \_ состоянием отрисовки D3DRS зенабле.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3D9Types. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Перечисления Direct3D](dx9-graphics-reference-d3d-enums.md)
</dt> <dt>

[**D3DRENDERSTATETYPE**](./d3drenderstatetype.md)
</dt> </dl>

 

 
