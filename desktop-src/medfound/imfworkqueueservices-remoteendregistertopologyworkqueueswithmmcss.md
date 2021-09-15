---
description: 'Версия метода Имфворккуеуесервицес:: Ендрегистертопологиворккуеуесвисммксс, поддерживающая удаленное взаимодействие.'
ms.assetid: 94dce412-6a72-4ddf-86a3-5176ee1eb6d2
title: Ремотиндрегистертопологиворккуеуесвисммксс (Мфобжектс. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3333becfcd7a3c5e2621b628b6435b96af017cf8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469282"
---
# <a name="remoteendregistertopologyworkqueueswithmmcss"></a>ремотиндрегистертопологиворккуеуесвисммксс

Версия метода [**имфворккуеуесервицес:: ендрегистертопологиворккуеуесвисммксс**](/windows/desktop/api/mfidl/nf-mfidl-imfworkqueueservices-endregistertopologyworkqueueswithmmcss) , поддерживающая удаленное взаимодействие.

``` syntax
[call_as(EndRegisterTopologyWorkQueuesWithMMCSS)]
HRESULT RemoteEndRegisterTopologyWorkQueuesWithMMCSS(
    IUnknown *pResult
);
```

## <a name="remarks"></a>Remarks

Приложения не могут вызывать этот метод напрямую, и объекты не реализуют этот метод. Метод не отображается в таблице vtable для интерфейса. Если [**ендрегистертопологиворккуеуесвисммксс**](/windows/desktop/api/mfidl/nf-mfidl-imfworkqueueservices-endregistertopologyworkqueueswithmmcss) вызывается через границы процесса, то библиотека DLL прокси или заглушки Media Foundation преобразует вызов в вызов удаленного метода и затем преобразует его обратно.

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

 

 




