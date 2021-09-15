---
description: 'Метод ID3DXMATRIXStack:: Скалелокал (D3DX10. h) — масштабирование текущей матрицы относительно источника объекта.'
ms.assetid: 748fce3a-a33c-4975-bbf0-dd3167a036f1
title: 'Метод ID3DXMATRIXStack:: Скалелокал (D3DX10. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXMATRIXStack.ScaleLocal
api_type:
- COM
api_location:
- D3DX10.lib
- D3DX10.dll
ms.openlocfilehash: 3961db0794703e3974dbd92d8eae8293173c2354
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462443"
---
# <a name="id3dxmatrixstackscalelocal-method-d3dx10h"></a>Метод ID3DXMATRIXStack:: Скалелокал (D3DX10. h)

Масштабировать текущую матрицу относительно источника объекта.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT ScaleLocal(
  [in] FLOAT x,
  [in] FLOAT y,
  [in] FLOAT z
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*x* \[ в\]
</dt> <dd>

Тип: **[ **float**](../winprog/windows-data-types.md)**

Компонент масштабирования по оси x.

</dd> <dt>

*y* \[ в\]
</dt> <dd>

Тип: **[ **float**](../winprog/windows-data-types.md)**

Компонент масштабирования в направлении y.

</dd> <dt>

*z* \[ в\]
</dt> <dd>

Тип: **[ **float**](../winprog/windows-data-types.md)**

Компонент масштабирования в направлении z.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если метод выполнен успешно, возвращается значение D3D \_ ОК.

## <a name="remarks"></a>Remarks

Этот метод Left — Умножает текущую матрицу на вычисленную матрицу масштабирования. Преобразование относится к локальному источнику объекта.


```
D3DXMATRIX tmp;
D3DXMatrixScaling(&tmp, x, y, z);
m_stack[m_currentPos] = tmp * m_stack[m_currentPos];
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX10. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>D3DX10. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[ID3DXMatrixStack](d3d10-id3dxmatrixstack.md)
</dt> <dt>

[Интерфейсы D3DX](d3d10-graphics-reference-d3dx10-interfaces.md)
</dt> </dl>

 

 
