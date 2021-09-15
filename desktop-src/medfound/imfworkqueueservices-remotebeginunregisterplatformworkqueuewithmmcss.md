---
description: 'Версия метода Имфворккуеуесервицес:: Бегинунрегистерплатформворккуеуевисммксс, поддерживающая удаленное взаимодействие.'
ms.assetid: c3117086-268e-4e52-acfb-2c8167adaa07
title: Ремотебегинунрегистерплатформворккуеуевисммксс (Мфобжектс. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3ab364f041d6bc8d0f6275879c82a937e98f463b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469288"
---
# <a name="remotebeginunregisterplatformworkqueuewithmmcss"></a>ремотебегинунрегистерплатформворккуеуевисммксс

Версия метода [**имфворккуеуесервицес:: бегинунрегистерплатформворккуеуевисммксс**](/windows/desktop/api/mfidl/nf-mfidl-imfworkqueueservices-beginunregisterplatformworkqueuewithmmcss) , поддерживающая удаленное взаимодействие.

``` syntax
[call_as(BeginUnregisterPlatformWorkQueueWithMMCSS)]
HRESULT RemoteBeginUnregisterPlatformWorkQueueWithMMCSS(
    DWORD dwPlatformWorkQueue,
    IMFRemoteAsyncCallback *pCallback
);
```

## <a name="remarks"></a>Remarks

Приложения не могут вызывать этот метод напрямую, и объекты не реализуют этот метод. Метод не отображается в таблице vtable для интерфейса. Если [**бегинунрегистерплатформворккуеуевисммксс**](/windows/desktop/api/mfidl/nf-mfidl-imfworkqueueservices-beginunregisterplatformworkqueuewithmmcss) вызывается через границы процесса, то библиотека DLL прокси или заглушки Media Foundation преобразует вызов в вызов удаленного метода и затем преобразует его обратно.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Мфобжектс. h (включение Мфидл. h)</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>Мфууид. lib</dt> </dl>                    |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**имфворккуеуесервицес**](/windows/desktop/api/mfidl/nn-mfidl-imfworkqueueservices)
</dt> </dl>

 

 




