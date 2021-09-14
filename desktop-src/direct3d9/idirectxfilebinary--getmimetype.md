---
description: Извлекает тип MIME для двоичных данных. Не рекомендуется.
ms.assetid: 57c42ace-4313-40d8-9992-eaf12edf3a30
title: 'Метод Идиректксфилебинари:: Жетмиметипе (Дксфиле. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IDirectXFileBinary.GetMimeType
api_type:
- COM
api_location:
- D3dxof.lib
- D3dxof.dll
ms.openlocfilehash: 965006dc6fbad1176307341a19fd1f186e670104
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168483"
---
# <a name="idirectxfilebinarygetmimetype-method"></a>Метод Идиректксфилебинари:: Жетмиметипе

Извлекает тип MIME для двоичных данных. Не рекомендуется.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetMimeType(
  [out] LPCSTR *pszMimeType
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*псзмиметипе* \[ заполняет\]
</dt> <dd>

Тип: **[ **LPCSTR**](../winprog/windows-data-types.md)\***

Адрес указателя для получения строки типа MIME.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если метод выполнен успешно, возвращается значение ДКСФИЛЕ \_ ОК. В случае сбоя метода возвращаемое значение может быть ДКСФИЛИРР \_ бадвалуе.

## <a name="remarks"></a>Remarks

Если в файле DirectX для двоичного объекта не указан тип MIME, функция устанавливает Псзмиметипе в **значение NULL**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Дксфиле. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>D3dxof. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[идиректксфилебинари](idirectxfilebinary.md)
</dt> </dl>

 

 
