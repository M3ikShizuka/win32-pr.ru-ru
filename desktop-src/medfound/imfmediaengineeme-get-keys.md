---
description: Возвращает объект ключей мультимедиа, связанный с обработчиком мультимедиа, или значение null, если отсутствует объект ключей мультимедиа.
ms.assetid: e6556a02-445d-4436-80de-e4156d6a3d63
title: 'Метод Имфмедиаенгиниме:: get_Keys'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMFMediaEngineEME.get_Keys
api_type:
- COM
api_location:
- mfmediaengine.h
ms.openlocfilehash: dcb06352065b28739a616a9f2216c20eedebb913
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127579974"
---
# <a name="imfmediaengineemeget_keys-method"></a>Метод Имфмедиаенгиниме:: Get \_ Keys

Возвращает объект ключей мультимедиа, связанный с обработчиком мультимедиа, или **значение NULL** , если отсутствует объект ключей мультимедиа.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_Keys(
   IMFMediaKeys **keys
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ключ* 
</dt> <dd>

Объект ключей мультимедиа, связанный с обработчиком мультимедиа, или **значение NULL** , если отсутствует объект ключей мультимедиа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                                      |
| IDL<br/>                      | <dl> <dt>Мфмедиаенгине. idl</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**имфмедиаенгиниме**](/windows/desktop/api/mfmediaengine/nn-mfmediaengine-imfmediaengineeme)
</dt> </dl>

 

 




