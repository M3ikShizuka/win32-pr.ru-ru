---
description: 'Версия метода Имфпмфост:: Креатеобжектбиклсид, поддерживающая удаленное взаимодействие.'
ms.assetid: be96be6d-47de-4d2b-81fc-13079de33888
title: Ремотекреатеобжектбиклсид (Мфобжектс. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9e57307ece851484675d01a699037647efad771d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127257915"
---
# <a name="remotecreateobjectbyclsid"></a>ремотекреатеобжектбиклсид

Версия метода [**имфпмфост:: креатеобжектбиклсид**](/windows/desktop/api/mfidl/nf-mfidl-imfpmphost-createobjectbyclsid) , поддерживающая удаленное взаимодействие.

``` syntax
[call_as(CreateObjectByCLSID)]
HRESULT RemoteCreateObjectByCLSID( 
    REFCLSID clsid,
    BYTE *pbData, 
    DWORD cbData, 
    REFIID riid,
    void **ppv
);
```

## <a name="remarks"></a>Комментарии

Приложения не могут вызывать этот метод напрямую, и объекты не реализуют этот метод. Метод не отображается в таблице vtable для интерфейса. Если [**креатеобжектбиклсид**](/windows/desktop/api/mfidl/nf-mfidl-imfpmphost-createobjectbyclsid) вызывается через границы процесса, то библиотека DLL прокси или заглушки Media Foundation преобразует вызов в вызов удаленного метода и затем преобразует его обратно.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Мфобжектс. h (включение Мфидл. h)</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>Мфууид. lib</dt> </dl>                    |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**имфпмфост**](/windows/desktop/api/mfidl/nn-mfidl-imfpmphost)
</dt> <dt>

[Сеанс PMP мультимедиа](pmp-media-session.md)
</dt> <dt>

[Путь к защищенному носителю](protected-media-path.md)
</dt> </dl>

 

 




