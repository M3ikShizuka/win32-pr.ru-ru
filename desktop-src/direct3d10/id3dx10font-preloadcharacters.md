---
description: Загрузка последовательности символов в видеопамять для повышения эффективности отрисовки на устройстве.
ms.assetid: 935a6248-e6b7-4fce-aaa7-b7f0c94c1f79
title: 'ID3DX10Font: метод:P Релоадчарактерс (D3DX10. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DX10Font.PreloadCharacters
api_type:
- COM
api_location:
- D3DX10.lib
- D3DX10.dll
ms.openlocfilehash: c4a6c0ac515457aee430dea7cc3f785ed2832aed5c566f84b9d4ee262ba8b5cf
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119953574"
---
# <a name="id3dx10fontpreloadcharacters-method"></a>ID3DX10Font: метод:P Релоадчарактерс

Загрузка последовательности символов в видеопамять для повышения эффективности отрисовки на устройстве.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT PreloadCharacters(
  [in] UINT First,
  [in] UINT Last
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Сначала* \[ окне\]
</dt> <dd>

Тип: **[ **uint**](../winprog/windows-data-types.md)**

Идентификатор первого символа, загружаемого в видеопамять.

</dd> <dt>

*Последний раз* \[ окне\]
</dt> <dd>

Тип: **[ **uint**](../winprog/windows-data-types.md)**

Идентификатор последнего символа, который должен быть загружен в видеопамять.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если метод выполнен успешно, возвращается значение S \_ . В случае сбоя метода возвращаемое значение может быть одним из следующих: D3DERR \_ инвалидкалл, D3DXERR \_ INVALIDDATA.

## <a name="remarks"></a>Remarks

Этот метод создает текстуры, содержащие глифы, представляющие входные символы. Глифы рисуются в виде ряда треугольников.

Символы не будут подготавливаться к просмотру на устройстве; ID3DX10Font: для отрисовки символов необходимо по-прежнему вызывать метод:D Равтекст. Однако предварительная загрузка символов в видеопамять ID3DX10Font::D Равтекст будет использовать значительно меньше ресурсов ЦП.

Этот метод внутренне преобразует символы в глифы с помощью функции GDI [жетчарактерплацемент](/previous-versions//ms534004(v=vs.85)).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX10. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>D3DX10. lib</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[ID3DX10Font](id3dx10font.md)
</dt> <dt>

[Интерфейсы D3DX](d3d10-graphics-reference-d3dx10-interfaces.md)
</dt> </dl>

 

 
