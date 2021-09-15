---
description: Позволяет процессу открывать общий ресурс или отключать процесс от открытия общих ресурсов.
ms.assetid: 5fa2b88f-e946-436c-953e-04e0e338146c
title: D3DAUTHENTICATEDCONFIGURE_SHAREDRESOURCE (D3d9types. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DAUTHENTICATEDCONFIGURE_SHAREDRESOURCE
api_type:
- HeaderDef
api_location:
- d3d9types.h
ms.openlocfilehash: 7404a4bed3ac3b1d4002bb03c45d7732500b77e4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570634"
---
# <a name="d3dauthenticatedconfigure_sharedresource"></a>D3DAUTHENTICATEDCONFIGURE \_ шаредресаурце

Позволяет процессу открывать общий ресурс или отключать процесс от открытия общих ресурсов.



| Требование | Значение |
|--------------|-------------------------------------------------------------------------------------------------------------|
| Идентификатор GUID команды | **D3DAUTHENTICATEDCONFIGURE \_ шаредресаурце**                                                               |
| Входные данные   | [**D3DAUTHENTICATEDCHANNEL \_ конфигурешаредресаурце**](d3dauthenticatedchannel-configuresharedresource.md) |



 

## <a name="remarks"></a>Remarks

Этот запрос поддерживают следующие типы каналов:

-   **\_Драйвер D3DAUTHENTICATEDCHANNEL \_ d3d9**
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

 

 




