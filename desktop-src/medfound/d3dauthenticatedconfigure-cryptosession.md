---
description: Связывает сеанс шифрования с устройством декодера DirectX Video Acceleration 2 (ДКСВА-2) и устройством Direct3D.
ms.assetid: d40fead7-8a86-426e-933e-13df21cdf50b
title: D3DAUTHENTICATEDCONFIGURE_CRYPTOSESSION (D3d9types. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DAUTHENTICATEDCONFIGURE_CRYPTOSESSION
api_type:
- HeaderDef
api_location:
- d3d9types.h
ms.openlocfilehash: 4b6fda19aef9629214aaa410fd43c4d64f16dd29
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127248578"
---
# <a name="d3dauthenticatedconfigure_cryptosession"></a>D3DAUTHENTICATEDCONFIGURE \_ CRYPTOSESSION

Связывает сеанс шифрования с устройством декодера DirectX Video Acceleration 2 (ДКСВА-2) и устройством Direct3D.



| Требование | Значение |
|--------------|-----------------------------------------------------------------------------------------------------------|
| Идентификатор GUID команды | **D3DAUTHENTICATEDCONFIGURE \_ CRYPTOSESSION**                                                              |
| Входные данные   | [**D3DAUTHENTICATEDCHANNEL \_ конфигурекриптосессион**](d3dauthenticatedchannel-configurecryptosession.md) |



 

## <a name="remarks"></a>Remarks

После отправки этой команды можно отправить запрос [D3DAUTHENTICATEDQUERY \_ аутпутид](d3dauthenticatedquery-outputid.md) , чтобы узнать, какие выходные данные видео связаны с сеансом шифрования.

Эта команда поддерживается следующими типами каналов:

-   **D3DAUTHENTICATEDCHANNEL \_ d3d9**
-   **\_ \_ Программное обеспечение драйвера D3DAUTHENTICATEDCHANNEL**

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>D3d9types. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Защита содержимого команды](content-protection-commands.md)
</dt> <dt>

[Защита содержимого на основе GPU](gpu-based-content-protection.md)
</dt> <dt>

[**IDirect3DAuthenticatedChannel9:: Configure**](/windows/desktop/api/d3d9/nf-d3d9-idirect3dauthenticatedchannel9-configure)
</dt> </dl>

 

 




