---
description: Передает значение ключа со всеми связанными данными, необходимыми модулю расшифровки содержимого для заданной ключевой системы.
ms.assetid: 29e66037-5f18-4724-b6f2-d85555e6af69
title: 'Метод Имфмедиакэйсессион:: Update'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMFMediaKeySession.Update
api_type:
- COM
api_location:
- mfmediaengine.h
ms.openlocfilehash: 15bc06523f0cf9a7dc433381dd596cea89608ce7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462217"
---
# <a name="imfmediakeysessionupdate-method"></a>Метод Имфмедиакэйсессион:: Update

Передает значение ключа со всеми связанными данными, необходимыми модулю расшифровки содержимого для заданной ключевой системы.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Update(
   const BYTE  *key,
         DWORD cb
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*key* 
</dt> <dd></dd> <dt>

*CB* 
</dt> <dd>

Число в байтах *ключа*.

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

[**имфмедиакэйсессион**](/windows/desktop/api/mfmediaengine/nn-mfmediaengine-imfmediakeysession)
</dt> </dl>

 

 




