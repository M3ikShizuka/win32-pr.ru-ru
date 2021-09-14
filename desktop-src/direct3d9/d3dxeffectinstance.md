---
description: Тип данных для управления набором параметров эффектов по умолчанию.
ms.assetid: a3408c0b-b4a6-47b1-b12e-594c13bd3a7d
title: Структура D3DXEFFECTINSTANCE (D3dx9mesh. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXEFFECTINSTANCE
api_type:
- HeaderDef
api_location:
- d3dx9mesh.h
ms.openlocfilehash: 6874da0fd04b34036152d58e94b16006e185e117
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066282"
---
# <a name="d3dxeffectinstance-structure"></a>Структура D3DXEFFECTINSTANCE

Тип данных для управления набором параметров эффектов по умолчанию.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct D3DXEFFECTINSTANCE {
  LPSTR               pEffectFilename;
  DWORD               NumDefaults;
  LPD3DXEFFECTDEFAULT pDefaults;
} D3DXEFFECTINSTANCE, *LPD3DXEFFECTINSTANCE;
```



## <a name="members"></a>Участники

<dl> <dt>

**пеффектфиленаме**
</dt> <dd>

Тип: **LPSTR**

</dd> <dd>

Имя файла действия.

</dd> <dt>

**нумдефаултс**
</dt> <dd>

Тип: **[ **DWORD**](../winprog/windows-data-types.md)**

</dd> <dd>

Количество параметров по умолчанию.

</dd> <dt>

**пдефаултс**
</dt> <dd>

Тип: **[ **LPD3DXEFFECTDEFAULT**](d3dxeffectdefault.md)**

</dd> <dd>

Указатель на массив элементов [**D3DXEFFECTDEFAULT**](d3dxeffectdefault.md) , каждый из которых содержит параметр Effect.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3dx9mesh. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Структуры эффектов](dx9-graphics-reference-effects-structures.md)
</dt> </dl>

 

 
