---
description: Применяет переплет к объекту ID3DXPRTBuffer buffer.
ms.assetid: db09aa50-3175-4588-8433-dad6bd37cf0c
title: 'Метод ID3DXTextureGutterHelper:: Апплигуттерспрт (D3DX9Mesh. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXTextureGutterHelper.ApplyGuttersPRT
api_type:
- COM
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 0fcfb4829774dc4fc754b566f531d6e4aff76751ae2d7eb13bc17e0c434b9cff
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119674644"
---
# <a name="id3dxtexturegutterhelperapplyguttersprt-method"></a>Метод ID3DXTextureGutterHelper:: Апплигуттерспрт

Применяет переплет к объекту [**ID3DXPRTBuffer**](id3dxprtbuffer.md) buffer.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT ApplyGuttersPRT(
  [in] LPD3DXPRTBUFFER pBuffer
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pBuffer* \[ окне\]
</dt> <dd>

Тип: **[ **LPD3DXPRTBUFFER**](id3dxprtbuffer.md)**

Указатель на объект буфера [**ID3DXPRTBuffer**](id3dxprtbuffer.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если метод выполнен успешно, возвращается значение S \_ . Если метод завершается с ошибкой, будет возвращено следующее значение. D3DERR \_ инвалидкалл

## <a name="remarks"></a>Remarks

[**Класс 2 пикселей текстуры**](id3dxtexturegutterhelper.md) создается путем повторной выборки класса 1 и 4 пикселей текстуры.

Ширина и высота текстуры должны совпадать с шириной и высотой, возвращаемой [**ID3DXTextureGutterHelper:: полуширинные**](id3dxtexturegutterhelper--getwidth.md) и [**ID3DXTextureGutterHelper:: Height**](id3dxtexturegutterhelper--getheight.md).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Mesh. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>   |



## <a name="see-also"></a>См. также

<dl> <dt>

[ID3DXTextureGutterHelper](id3dxtexturegutterhelper.md)
</dt> </dl>

 

 




