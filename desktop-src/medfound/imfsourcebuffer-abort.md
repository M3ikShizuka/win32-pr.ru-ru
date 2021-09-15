---
description: Прерывает обработку текущего сегмента мультимедиа.
ms.assetid: 31253d0d-c53f-47bd-823a-fc564cb63b78
title: 'Метод Имфсаурцебуффер:: Abort'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMFSourceBuffer.Abort
api_type:
- COM
api_location:
- mfmediaengine.h
ms.openlocfilehash: 3a8b5115032fb918af66094bb87c7118eb503da3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572851"
---
# <a name="imfsourcebufferabort-method"></a>Метод Имфсаурцебуффер:: Abort

Прерывает обработку текущего сегмента мультимедиа.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Abort();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

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

[**имфсаурцебуффер**](/windows/desktop/api/mfmediaengine/nn-mfmediaengine-imfsourcebuffer)
</dt> </dl>

 

 




