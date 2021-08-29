---
description: Создает объект Font. примечание. вместо использования этой функции рекомендуется использовать DirectWrite и библиотеку директкстк, класс спритефонт.
ms.assetid: 057ee033-37d8-4fc1-9f35-776393fff008
title: Функция D3DX10CreateFontIndirect (D3DX10Core. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DX10CreateFontIndirect
api_type:
- LibDef
api_location:
- D3DX10.lib
- D3DX10.dll
ms.openlocfilehash: bfbbc2cdb0e8aad5851de40312bd7d646eb9e3af22e71f0638a7fa1e52f342f3
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119989154"
---
# <a name="d3dx10createfontindirect-function"></a>Функция D3DX10CreateFontIndirect

Создает объект Font.

> [!Note]  
> вместо использования этой функции рекомендуется использовать [DirectWrite](../directwrite/direct-write-portal.md) и библиотеку [директкстк](https://github.com/Microsoft/DirectXTK) , класс **спритефонт** .

 

## <a name="syntax"></a>Синтаксис


```C++
HRESULT D3DX10CreateFontIndirect(
  _In_        ID3D10Device     *pDevice,
  _In_  const D3DX10_FONT_DESC *pDesc,
  _Out_       LPD3DX10FONT     *ppFont
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пдевице* \[ окне\]
</dt> <dd>

Тип: **[ **ID3D10Device**](/windows/desktop/api/D3D10/nn-d3d10-id3d10device)\***

Указатель на интерфейс интерфейса [**ID3D10Device**](/windows/desktop/api/D3D10/nn-d3d10-id3d10device) .

</dd> <dt>

*пдеск* \[ окне\]
</dt> <dd>

Тип: **const [**D3DX10 \_ Font \_ DESC**](d3dx10-font-desc.md) \***

Указатель на [**D3DX10 структуру \_ шрифта \_**](d3dx10-font-desc.md) с описанием атрибутов создаваемого объекта Font. Если определен Юникод, вызов функции разрешается в D3DXCreateFontIndirectW. В противном случае вызов функции разрешается в D3DXCreateFontIndirectA, так как используются строки ANSI.

</dd> <dt>

*ппфонт* \[ заполняет\]
</dt> <dd>

Тип: **[ **LPD3DX10FONT**](id3dx10font.md)\***

Возвращает указатель на [**интерфейс ID3DX10Font**](id3dx10font.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Возвращаемое значение является одним из значений, перечисленных в [кодах возврата Direct3D 10](d3d10-graphics-reference-returnvalues.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX10Core. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3DX10. lib</dt> </dl>   |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Функции общего назначения](d3d10-graphics-reference-d3dx10-functions-general-purpose.md)
</dt> </dl>

 

 
