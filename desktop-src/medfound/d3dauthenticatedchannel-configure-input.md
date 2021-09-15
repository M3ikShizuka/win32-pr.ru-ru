---
description: 'Содержит входные данные для метода IDirect3DAuthenticatedChannel9:: Configure.'
ms.assetid: 7646100e-f768-4935-9e71-1d9db0d69c52
title: Структура D3DAUTHENTICATEDCHANNEL_CONFIGURE_INPUT (D3d9types. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DAUTHENTICATEDCHANNEL_CONFIGURE_INPUT
api_type:
- HeaderDef
api_location:
- d3d9types.h
ms.openlocfilehash: 82cd60dbb65517beb65a3a7cb413e1d93ac72062
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572863"
---
# <a name="d3dauthenticatedchannel_configure_input-structure"></a>D3DAUTHENTICATEDCHANNEL \_ Настройка \_ входной структуры

Содержит входные данные для метода [**IDirect3DAuthenticatedChannel9:: Configure**](/windows/desktop/api/d3d9/nf-d3d9-idirect3dauthenticatedchannel9-configure) .

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _D3DAUTHENTICATEDCHANNEL_CONFIGURE_INPUT {
  D3D_OMAC omac;
  GUID     ConfigureType;
  HANDLE   hChannel;
  UINT     SequenceNumber;
} D3DAUTHENTICATEDCHANNEL_CONFIGURE_INPUT;
```



## <a name="members"></a>Участники

<dl> <dt>

**омак**
</dt> <dd>

Структура [**D3D \_ ОМАК**](d3d-omac.md) , содержащая код проверки подлинности сообщения (Mac) данных. Для вычисления этого значения в блоке данных, который отображается после этого элемента структуры, драйвер использует одноключовый CBC MAC (ОМАК) на основе AES.

</dd> <dt>

**конфигуретипе**
</dt> <dd>

Идентификатор GUID, указывающий команду. Список значений см. в разделе [Защита содержимого Commands](content-protection-commands.md).

</dd> <dt>

**хчаннел**
</dt> <dd>

Маркер для аутентифицированного канала. Чтобы получить этот маркер, вызовите метод [**IDirect3DDevice9Video:: креатеаусентикатедчаннел**](/windows/desktop/api/d3d9/nf-d3d9-idirect3ddevice9video-createauthenticatedchannel).

</dd> <dt>

**SequenceNumber**
</dt> <dd>

Порядковый номер запроса. В начале сеанса создайте криптографически защищенное 32-разрядное случайное число, которое будет использоваться в качестве начального порядкового номера. Для каждой команды увеличьте порядковый номер на 1.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>D3d9types. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Видеоструктуры Direct3D](direct3d-video-structures.md)
</dt> <dt>

[**IDirect3DAuthenticatedChannel9:: Configure**](/windows/desktop/api/d3d9/nf-d3d9-idirect3dauthenticatedchannel9-configure)
</dt> </dl>

 

 




