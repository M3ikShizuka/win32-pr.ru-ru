---
title: Структура XMUINT4
description: Описывает вектор целого числа без знака 4D.
ms.assetid: 289293e5-882e-479c-886e-82c802f824b5
keywords:
- HLSL структура XMUINT4
topic_type:
- apiref
api_name:
- XMUINT4
api_location:
- D3DX_DXGIFormatConvert.inl
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5e424b4e5fd1c97f5aec01571d887b54dbb143b7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126966413"
---
# <a name="xmuint4-structure"></a>Структура XMUINT4

Описывает вектор целого числа без знака 4D.

## <a name="syntax"></a>Синтаксис


``` syntax
typedef struct _XMUINT4 {
  UINT x;
  UINT {
    UINT {
      UINT w;
    }z;
  }y;
} XMUINT4;
```



## <a name="members"></a>Участники

<dl> <dt>

**x**
</dt> <dd>

компонент x вектора.

</dd> <dt>

**y**
</dt> <dd>

y-компонент вектора.

<dl> <dt>

**z**
</dt> <dd>

z-компонент вектора.

<dl> <dt>

**w**
</dt> <dd>

w — компонент вектора.

</dd> </dl> </dd> </dl> </dd> </dl>




## <a name="remarks"></a>Комментарии

Эта структура определена в ``D3DX\_DXGIFormatConvert.inl`` заголовке пакета SDK DirectX (июнь 2010) для использования из C++. последняя версия этого заголовка в пакете [Microsoft. дкссдк. D3DX](https://www.nuget.org/packages/Microsoft.DXSDK.D3DX) NuGet больше не определяет его и использует [DirectX:: XMUINT4](/windows/win32/api/directxmath/ns-directxmath-xmuint4) в директксмас.




## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|--------------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3DX \_ дксгиформатконверт. inl</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Структуры](format-conversion-structures.md)
</dt> <dt>

[Распаковка и \_ формат упаковки для редактирования образа In-Place](dx-graphics-hlsl-unpacking-packing-dxgi-format.md)
</dt> </dl>