---
description: Описывает ключ кватернион для использования в анимации по ключевым кадрам. Ключ кватернион — это значение кватерниона в заданный момент времени.
ms.assetid: 8f5b74a3-f712-40ac-942c-a2189c2327c8
title: Структура D3DXKEY_QUATERNION (D3dx9anim. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXKEY_QUATERNION
api_type:
- HeaderDef
api_location:
- d3dx9anim.h
ms.openlocfilehash: 12e4deead606c1a2c5b103ed9fd0e31e23515982
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126966758"
---
# <a name="d3dxkey_quaternion-structure"></a>\_Структура КВАТЕРНИОНА D3DXKEY

Описывает ключ кватернион для использования в анимации по ключевым кадрам. Ключ кватернион — это значение кватерниона в заданный момент времени.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct D3DXKEY_QUATERNION {
  FLOAT          Time;
  D3DXQUATERNION Value;
} D3DXKEY_QUATERNION, *LPD3DXKEY_QUATERNION;
```



## <a name="members"></a>Участники

<dl> <dt>

**Время**
</dt> <dd>

Тип: **[ **float**](../winprog/windows-data-types.md)**

</dd> <dd>

Значение времени.

</dd> <dt>

**Значение**
</dt> <dd>

Тип: **[ **D3DXQUATERNION**](d3dxquaternion.md)**

</dd> <dd>

[**D3DXQUATERNION**](d3dxquaternion.md) кватернион, предоставляющий значения поворота.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3dx9anim. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Структуры D3DX](dx9-graphics-reference-d3dx-structures.md)
</dt> </dl>

 

 
