---
description: Задает координаты текстуры (u, v) каждого шаг текселя.
ms.assetid: b1f8f5d6-568f-4868-87c9-9d6b1034d898
title: 'Метод ID3DXTextureGutterHelper:: Сеттекселмап (D3DX9Mesh. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXTextureGutterHelper.SetTexelMap
api_type:
- COM
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 7c95ca7bff03cdd44e5bd5a331c696534e9a9ad43deacc49c181eb97fbc5ee9d
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119491934"
---
# <a name="id3dxtexturegutterhelpersettexelmap-method"></a>Метод ID3DXTextureGutterHelper:: Сеттекселмап

Задает координаты текстуры (u, v) каждого шаг текселя.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetTexelMap(
  [in] D3DXVECTOR2 *pTexelData
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*птекселдата* \[ окне\]
</dt> <dd>

Тип: **[ **D3DXVECTOR2**](d3dxvector2.md)\***

Указатель на расположение в координатах текстуры (u, v), где размещается каждая шаг текселя.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если метод выполнен успешно, возвращается значение S \_ . Если метод завершается с ошибкой, будет возвращено следующее значение. D3DERR \_ инвалидкалл

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Mesh. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>   |



## <a name="see-also"></a>См. также

<dl> <dt>

[ID3DXTextureGutterHelper](id3dxtexturegutterhelper.md)
</dt> </dl>

 

 




