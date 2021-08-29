---
description: Возвращает интерфейс ID3DXFile объекта, который создал этот объект ID3DXFileSaveObject.
ms.assetid: 79249d17-cae3-43d9-9ccb-fa804b02a353
title: Метод ID3DXFileSaveObject::-File (D3DX9Xof. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXFileSaveObject.GetFile
api_type:
- COM
api_location:
- D3dx9.lib
- D3dx9.dll
ms.openlocfilehash: 3f46344244405aca80789ae45db172e7693c6a01f77a014737a90080c1e3f21c
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119121198"
---
# <a name="id3dxfilesaveobjectgetfile-method"></a>Метод ID3DXFileSaveObject:: onfile

Возвращает интерфейс [**ID3DXFile**](id3dxfile.md) объекта, который создал этот объект [**ID3DXFileSaveObject**](id3dxfilesaveobject.md) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetFile(
  [in] ID3DXFile ppFile
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппфиле* \[ окне\]
</dt> <dd>

Тип: **[ **ID3DXFile**](id3dxfile.md)**

Адрес указателя на объект [**ID3DXFile**](id3dxfile.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если метод выполнен успешно, возвращается значение S \_ . В случае сбоя метода возвращаемое значение может быть одним из следующих: D3DXFERR \_ бадвалуе, e \_ Interface, e \_ указатель.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Xof. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>  |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[ID3DXFileSaveObject](id3dxfilesaveobject.md)
</dt> </dl>

 

 




