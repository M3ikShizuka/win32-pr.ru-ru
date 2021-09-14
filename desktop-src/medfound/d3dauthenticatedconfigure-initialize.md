---
description: Инициализирует аутентифицированный канал.
ms.assetid: a74edbaa-af57-4f8e-9974-f6053f59377f
title: D3DAUTHENTICATEDCONFIGURE_INITIALIZE (D3d9types. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DAUTHENTICATEDCONFIGURE_INITIALIZE
api_type:
- HeaderDef
api_location:
- d3d9types.h
ms.openlocfilehash: 2cd3238b7a7eea27356ce76ec9c83bf8aea4d7f0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127248572"
---
# <a name="d3dauthenticatedconfigure_initialize"></a>\_Инициализация D3DAUTHENTICATEDCONFIGURE

Инициализирует аутентифицированный канал.



| Требование | Значение |
|--------------|-----------------------------------------------------------------------------------------------------|
| Идентификатор GUID команды | **\_Инициализация D3DAUTHENTICATEDCONFIGURE**                                                           |
| Входные данные   | [**D3DAUTHENTICATEDCHANNEL \_ конфигуреинитиализе**](d3dauthenticatedchannel-configureinitialize.md) |



 

## <a name="remarks"></a>Remarks

Отправить эту команду один раз в начале сеанса. Эту команду можно отправить только один раз для каждого канала, прошедшего проверку подлинности. Входной порядковый номер для этой команды не учитывается.

Эта команда поддерживается следующими типами каналов:

-   **\_Оборудование драйвера \_ D3DAUTHENTICATEDCHANNEL**
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

 

 




