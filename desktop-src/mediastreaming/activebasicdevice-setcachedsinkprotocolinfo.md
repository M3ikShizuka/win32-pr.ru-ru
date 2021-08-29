---
title: Метод Активебасикдевице Сеткачедсинкпротоколинфо (Плайтодевице. h)
description: Возвращает сведения о кэшированном протоколе приемника для устройства. | Метод Активебасикдевице Сеткачедсинкпротоколинфо (Плайтодевице. h)
ms.assetid: C4856B97-89F9-43EC-B778-9E0CDAAF2C47
keywords:
- API потоковой передачи мультимедиа метода Сеткачедсинкпротоколинфо
- API потоковой передачи мультимедиа метода Сеткачедсинкпротоколинфо, интерфейс Активебасикдевице
- API потоковой передачи мультимедиа интерфейса Активебасикдевице, метод Сеткачедсинкпротоколинфо
topic_type:
- apiref
api_name:
- ActiveBasicDevice.SetCachedSinkProtocolInfo
api_location:
- playtodevice.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4dfcfc780371f339b4fd14620975fc27e8dd08ed6ac9f054cfd2654840dc8022
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119952764"
---
# <a name="activebasicdevicesetcachedsinkprotocolinfo-method"></a>Метод Активебасикдевице:: Сеткачедсинкпротоколинфо

Возвращает сведения о кэшированном протоколе приемника для устройства.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetCachedSinkProtocolInfo(
  [in] GUID   physicalNetworkInterface,
  [in] UINT64 bitrate
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*фисикалнетворкинтерфаце* \[ окне\]
</dt> <dd>

Указывает физический сетевой интерфейс.

</dd> <dt>

*скорость* \[ окне\]
</dt> <dd>

Значение скорости.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                                     |
| Заголовок<br/>                   | <dl> <dt>Плайтодевице. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Плайтодевице. idl</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Playtodevice.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**активебасикдевице**](/previous-versions/windows/desktop/legacy/dn385755(v=vs.85))
</dt> </dl>

 

