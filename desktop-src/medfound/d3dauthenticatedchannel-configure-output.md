---
description: 'Содержит ответ на вызов метода IDirect3DAuthenticatedChannel9:: Configure.'
ms.assetid: 6f33d3f7-a883-4aca-a058-b656d745f2b1
title: Структура D3DAUTHENTICATEDCHANNEL_CONFIGURE_OUTPUT (D3d9types. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DAUTHENTICATEDCHANNEL_CONFIGURE_OUTPUT
api_type:
- HeaderDef
api_location:
- d3d9types.h
ms.openlocfilehash: 6c7a029bd73069795b83b0b2a330835782192683
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572859"
---
# <a name="d3dauthenticatedchannel_configure_output-structure"></a>D3DAUTHENTICATEDCHANNEL \_ Настройка \_ выходной структуры

Содержит ответ на вызов метода [**IDirect3DAuthenticatedChannel9:: Configure**](/windows/desktop/api/d3d9/nf-d3d9-idirect3dauthenticatedchannel9-configure) .

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _D3DAUTHENTICATEDCHANNEL_CONFIGURE_OUTPUT {
  D3D_OMAC omac;
  GUID     ConfigureType;
  HANDLE   hChannel;
  UINT     SequenceNumber;
  HRESULT  ReturnCode;
} D3DAUTHENTICATEDCHANNEL_CONFIGURE_OUTPUT;
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

Маркер для аутентифицированного канала.

</dd> <dt>

**SequenceNumber**
</dt> <dd>

Порядковый номер команды.

</dd> <dt>

**ReturnCode**
</dt> <dd>

Код результата для команды.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Для членов **конфигуретипе**, **хчаннел** и **SequenceNumber** драйвер использует те же значения, что и приложение, предоставленное в [**D3DAUTHENTICATEDCHANNEL \_ Настройка \_ входной**](d3dauthenticatedchannel-configure-input.md) структуры. Приложение должно проверить, совпадают ли эти значения.

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

 

 




