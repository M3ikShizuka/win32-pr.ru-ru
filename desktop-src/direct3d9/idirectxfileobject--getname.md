---
description: Получает указатель на имя объекта файла DirectX. Не рекомендуется.
ms.assetid: feb3faa2-22b9-47ed-8a38-33092821d484
title: Метод Идиректксфилеобжект::-Name (Дксфиле. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IDirectXFileObject.GetName
api_type:
- COM
api_location:
- D3dxof.lib
- D3dxof.dll
ms.openlocfilehash: e67381a26e3d0f1031e282d6530562416919e8cf52800a07301bf18820887828
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119846954"
---
# <a name="idirectxfileobjectgetname-method"></a>Метод Идиректксфилеобжект:: Name

Получает указатель на имя объекта файла DirectX. Не рекомендуется.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetName(
  [out]     LPSTR   pstrNameBuf,
  [in, out] LPDWORD pdwBufLen
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пстрнамебуф* \[ заполняет\]
</dt> <dd>

Тип: **[ **LPSTR**](../winprog/windows-data-types.md)**

Указатель на буфер, в который будет скопировано имя объекта файла DirectX. Задайте **значение NULL** , если требуется только длина буфера.

</dd> <dt>

*пдвбуфлен* \[ в, out\]
</dt> <dd>

Тип: **[ **лпдворд**](../winprog/windows-data-types.md)**

Указатель на DWORD, указывающий длину буфера, на который указывает Пстрнамебуф. Значение параметра Пдвбуфлен будет изменено на длину буфера, необходимую для хранения имени объекта, даже если Пстрнамебуф имеет **значение NULL**. В любом случае функция возвратит ДКСФИЛИРР \_ бадвалуе, если исходное значение пдвбуфлен не превышает длину, необходимую для хранения имени объекта.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если метод выполнен успешно, возвращается значение ДКСФИЛЕ \_ ОК. Если метод завершается с ошибкой, возвращаемое значение может быть одним из следующих значений. ДКСФИЛИРР \_ БАДАЛЛОК дксфилирр \_ бадвалуе

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Дксфиле. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>D3dxof. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[идиректксфилеобжект](idirectxfileobject.md)
</dt> </dl>

 

 
