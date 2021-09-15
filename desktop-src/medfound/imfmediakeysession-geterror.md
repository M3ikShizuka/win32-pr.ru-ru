---
description: Возвращает состояние ошибки, связанное с сеансом ключа мультимедиа.
ms.assetid: 4693b7d5-59ee-472f-83fc-1ecbcc165dac
title: 'Метод Имфмедиакэйсессион:: Error'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMFMediaKeySession.GetError
api_type:
- COM
api_location:
- mfmediaengine.h
ms.openlocfilehash: 4f0a42601698a9cd62dc6cb23ca9e69ac2cc8a49
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127580439"
---
# <a name="imfmediakeysessiongeterror-method"></a>Метод Имфмедиакэйсессион:: Error

Возвращает состояние ошибки, связанное с сеансом ключа мультимедиа.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetError(
   USHORT *code,
   DWORD  *systemCode
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*code* 
</dt> <dd>

Код ошибки.

</dd> <dt>

*системкоде* 
</dt> <dd>

Сведения об ошибках, специфичных для платформы.

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

 

 




