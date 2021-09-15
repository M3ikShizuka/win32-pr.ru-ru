---
description: Описывает таблицу Хаффмана контроллера домена JPEG.
ms.assetid: 9D6C18C3-F75C-41E0-9EFA-E882E89DE713
title: Структура DXGI_JPEG_DC_HUFFMAN_TABLE (Дксгитипе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DXGI_JPEG_DC_HUFFMAN_TABLE
api_type:
- HeaderDef
api_location:
- dxgitype.h
ms.openlocfilehash: b2f5f73f7c6def745b987818b9ec30fb3e2752e2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574051"
---
# <a name="dxgi_jpeg_dc_huffman_table-structure"></a>\_ \_ \_ Структура таблицы ХАФФМАНА DC для DXGI JPEG \_

Описывает таблицу Хаффмана контроллера домена JPEG.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct DXGI_JPEG_DC_HUFFMAN_TABLE {
  BYTE CodeCounts[12];
  BYTE CodeValues[12];
} DXGI_JPEG_DC_HUFFMAN_TABLE;
```



## <a name="members"></a>Участники

<dl> <dt>

**кодекаунтс**
</dt> <dd>

Количество кодов для каждой длины кода.

</dd> <dt>

**кодевалуес**
</dt> <dd>

Значения кода Хаффмана в порядке возрастания длины кода.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Дксгитипе. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Структуры DXGI](d3d10-graphics-reference-dxgi-structures.md)
</dt> </dl>

 

 




