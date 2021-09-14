---
title: Метод ID3DX11DataProcessor Креатедевицеобжект (D3DX11core. h)
description: обратите внимание, что библиотека служебной программы D3DX (D3DX 9, D3DX 10 и D3DX 11) является устаревшей для Windows 8 и не поддерживается для приложений магазина Windows. Создает объект устройства.
ms.assetid: 797d216b-2f54-4d24-aa97-04be0c71f909
keywords:
- Метод Креатедевицеобжект Direct3D 11
- Метод Креатедевицеобжект Direct3D 11, интерфейс ID3DX11DataProcessor
- Интерфейс ID3DX11DataProcessor Direct3D 11, метод Креатедевицеобжект
topic_type:
- apiref
api_name:
- ID3DX11DataProcessor.CreateDeviceObject
api_location:
- D3DX11.lib
- D3DX11.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f6ff178cec1830d1b0213af23a2a70654416d35e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172512"
---
# <a name="id3dx11dataprocessorcreatedeviceobject-method"></a>Метод ID3DX11DataProcessor:: Креатедевицеобжект

> [!Note]  
> библиотека служебной программы D3DX (D3DX 9, D3DX 10 и D3DX 11) является устаревшей для Windows 8 и не поддерживается для приложений магазина Windows.

 

Создает объект устройства.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT CreateDeviceObject(
  [out] void **ppDataObject
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппдатаобжект* \[ заполняет\]
</dt> <dd>

Тип: **void \* \***

Адрес указателя на созданный объект устройства.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Возвращаемое значение является одним из значений, перечисленных в [кодах возврата Direct3D 11](d3d11-graphics-reference-returnvalues.md).

## <a name="remarks"></a>Комментарии

Этот метод используется [**интерфейсом ID3DX11ThreadPump**](id3dx11threadpump.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX11core. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3DX11. lib</dt> </dl>   |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[ID3DX11DataProcessor](id3dx11dataprocessor.md)
</dt> <dt>

[Интерфейсы D3DX](d3d11-graphics-reference-d3dx11-interfaces.md)
</dt> </dl>

 

 





