---
description: Задает для .NET динамический код .NET CRL на диске.
ms.assetid: 4C8C3EF5-5C3C-4710-8223-D7B5BA86EF47
title: Функция Влдпсетдинамиккодетруст (Wldp. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- WldpSetDynamicCodeTrust
api_type:
- DllExport
api_location:
- wldp.dll
ms.openlocfilehash: 5a7277f13596ff3d397c97c8e8260e57e0e444e6943ba68f073f90c90cf3583d
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119075644"
---
# <a name="wldpsetdynamiccodetrust-function"></a>Функция Влдпсетдинамиккодетруст

Задает для .NET динамический код .NET CRL на диске.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT WINAPI WldpSetDynamicCodeTrust(
   HANDLE FileHandle
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*FileHandle* 
</dt> <dd>

Обработайте файл динамического кода на диске.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **значение \_ ОК** в случае успеха или код ошибки в противном случае.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1803\]<br/>                           |
| Минимальная версия сервера<br/> | Windows Server 2016 \[ только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Wldp. h</dt> </dl>   |
| DLL<br/>                      | <dl> <dt>Wldp.dll</dt> </dl> |



 

 




