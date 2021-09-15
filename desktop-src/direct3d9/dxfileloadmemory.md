---
description: Определяет данные памяти. Не рекомендуется.
ms.assetid: fe791e13-d5de-425f-b68f-80db8b332cc6
title: Структура ДКСФИЛЕЛОАДМЕМОРИ (Дксфиле. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DXFILELOADMEMORY
api_type:
- HeaderDef
api_location:
- DXFile.h
ms.openlocfilehash: 02424abd354811a6522b58dd0011ecdddce24564
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127457634"
---
# <a name="dxfileloadmemory-structure"></a>Структура ДКСФИЛЕЛОАДМЕМОРИ

Определяет данные памяти. Не рекомендуется.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct DXFILELOADMEMORY {
  LPVOID lpMemory;
  DWORD  dSize;
} DXFILELOADMEMORY, *LPDXFILELOADMEMORY;
```



## <a name="members"></a>Участники

<dl> <dt>

**лпмемори**
</dt> <dd>

Тип: **[ **лпвоид**](../winprog/windows-data-types.md)**

</dd> <dd>

Указатель на блок памяти для загрузки.

</dd> <dt>

**дсизе**
</dt> <dd>

Тип: **[ **DWORD**](../winprog/windows-data-types.md)**

</dd> <dd>

Размер блока памяти, который должен быть загружен, в байтах.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Эта структура определяет ресурс для загрузки, когда приложение использует метод [**креатинумобжект**](idirectxfile--createenumobject.md) и указывает дксфилелоад \_ фроммемори.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|-------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Дксфиле. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Структуры файлов X](dx9-graphics-reference-x-file-structures.md)
</dt> <dt>

[**креатинумобжект**](idirectxfile--createenumobject.md)
</dt> <dt>

[Константы ДКСФИЛЕ](dxfile.md)
</dt> </dl>

 

 
