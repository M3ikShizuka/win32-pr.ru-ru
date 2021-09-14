---
description: Описывает функцию, используемую в результате действия.
ms.assetid: 5d9deb82-7fe5-4408-8a6a-b34ecd97e8ba
title: Структура D3DXFUNCTION_DESC (D3dx9effect. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXFUNCTION_DESC
api_type:
- HeaderDef
api_location:
- d3dx9effect.h
ms.openlocfilehash: ec53cae4689ebc1795937012259b2e219630568b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066244"
---
# <a name="d3dxfunction_desc-structure"></a>\_Структура D3DXFUNCTION DESC

Описывает функцию, используемую в результате действия.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct D3DXFUNCTION_DESC {
  LPCSTR Name;
  UINT   Annotations;
} D3DXFUNCTION_DESC, *LPD3DXFUNCTION_DESC;
```



## <a name="members"></a>Участники

<dl> <dt>

**имя**;
</dt> <dd>

Тип: **[ **LPCSTR**](../winprog/windows-data-types.md)**

</dd> <dd>

Имя функции.

</dd> <dt>

**Примечания**
</dt> <dd>

Тип: **[ **uint**](../winprog/windows-data-types.md)**

</dd> <dd>

Не используется. Этому элементу всегда будет присвоено значение 0, [**жетфунктиондеск**](id3dxbaseeffect--getfunctiondesc.md).

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3dx9effect. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Структуры эффектов](dx9-graphics-reference-effects-structures.md)
</dt> </dl>

 

 
