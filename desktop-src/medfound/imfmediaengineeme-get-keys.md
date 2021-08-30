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
ms.openlocfilehash: 2df0be51eaf634879c2f8e90ae864b2e0dad5ce54271c55f5a81251141471843
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119942084"
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

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                                      |
| IDL<br/>                      | <dl> <dt>Мфмедиаенгине. idl</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**имфмедиаенгиниме**](/windows/desktop/api/mfmediaengine/nn-mfmediaengine-imfmediaengineeme)
</dt> </dl>

 

 




