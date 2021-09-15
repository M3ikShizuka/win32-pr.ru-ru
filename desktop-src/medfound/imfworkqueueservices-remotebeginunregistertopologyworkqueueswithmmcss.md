---
description: 'Версия метода Имфворккуеуесервицес:: Бегинунрегистертопологиворккуеуесвисммксс, поддерживающая удаленное взаимодействие.'
ms.assetid: 1a168462-400d-46c9-a489-7b861770469f
title: Ремотебегинунрегистертопологиворккуеуесвисммксс (Мфобжектс. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f52f82c55d692a2e1d9160c7a619338d82956ea0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469284"
---
# <a name="remotebeginunregistertopologyworkqueueswithmmcss"></a>ремотебегинунрегистертопологиворккуеуесвисммксс

Версия метода [**имфворккуеуесервицес:: бегинунрегистертопологиворккуеуесвисммксс**](/windows/desktop/api/mfidl/nf-mfidl-imfworkqueueservices-beginunregistertopologyworkqueueswithmmcss) , поддерживающая удаленное взаимодействие.

``` syntax
[call_as(BeginUnregisterTopologyWorkQueuesWithMMCSS)]
HRESULT RemoteBeginUnregisterTopologyWorkQueuesWithMMCSS(
    IMFRemoteAsyncCallback *pCallback
);
```

## <a name="remarks"></a>Remarks

Приложения не могут вызывать этот метод напрямую, и объекты не реализуют этот метод. Метод не отображается в таблице vtable для интерфейса. Если [**бегинунрегистертопологиворккуеуесвисммксс**](/windows/desktop/api/mfidl/nf-mfidl-imfworkqueueservices-beginunregistertopologyworkqueueswithmmcss) вызывается через границы процесса, то библиотека DLL прокси или заглушки Media Foundation преобразует вызов в вызов удаленного метода и затем преобразует его обратно.

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

 

 




