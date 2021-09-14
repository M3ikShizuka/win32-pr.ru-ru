---
description: Содержит входные данные для \_ запроса D3DAUTHENTICATEDQUERY CRYPTOSESSION.
ms.assetid: 3a4dead8-fe23-41b4-a167-e0430d09248a
title: Структура D3DAUTHENTICATEDCHANNEL_QUERYCRYPTOSESSION_INPUT (D3d9types. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DAUTHENTICATEDCHANNEL_QUERYCRYPTOSESSION_INPUT
api_type:
- HeaderDef
api_location:
- d3d9types.h
ms.openlocfilehash: 76b9d09bcb03dbf3742d551c253d3f4982215757
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461013"
---
# <a name="d3dauthenticatedchannel_querycryptosession_input-structure"></a>\_ \_ Входная структура D3DAUTHENTICATEDCHANNEL куерикриптосессион

Содержит входные данные для запроса [**D3DAUTHENTICATEDQUERY \_ CRYPTOSESSION**](d3dauthenticatedquery-cryptosession.md) .

Чтобы отправить этот запрос, вызовите метод [**IDirect3DAuthenticatedChannel9:: Query**](/windows/desktop/api/d3d9/nf-d3d9-idirect3dauthenticatedchannel9-query).

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _D3DAUTHENTICATEDCHANNEL_QUERYCRYPTOSESSION_INPUT {
  D3DAUTHENTICATEDCHANNEL_QUERY_INPUT Input;
  HANDLE                              DXVA2DecodeHandle;
} D3DAUTHENTICATEDCHANNEL_QUERYCRYPTOSESSION_INPUT;
```



## <a name="members"></a>Участники

<dl> <dt>

**Ввод**
</dt> <dd>

[**\_ \_ Входная Структура запроса D3DAUTHENTICATEDCHANNEL**](d3dauthenticatedchannel-query-input.md) , содержащая идентификатор GUID для запроса и других данных.

</dd> <dt>

**DXVA2DecodeHandle**
</dt> <dd>

Маркер устройства декодера DirectX Video Acceleration 2 (ДКСВА-2).

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

[**IDirect3DAuthenticatedChannel9:: Query**](/windows/desktop/api/d3d9/nf-d3d9-idirect3dauthenticatedchannel9-query)
</dt> </dl>

 

 




