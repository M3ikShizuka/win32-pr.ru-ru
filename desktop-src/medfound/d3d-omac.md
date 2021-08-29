---
description: Содержит код проверки подлинности сообщения (MAC).
ms.assetid: be5515fd-1936-46b8-9fc8-8d1f87048c38
title: Структура D3D_OMAC (D3d9types. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3D_OMAC
api_type:
- HeaderDef
api_location:
- d3d9types.h
ms.openlocfilehash: 05cf39bccc33eb1f993b0e86cfa89fc290832b422129441d99f028f3d826c3fd
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119449552"
---
# <a name="d3d_omac-structure"></a>\_Структура D3D ОМАК

Содержит код проверки подлинности сообщения (MAC).

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _D3D_OMAC {
  BYTE Omac[D3D_OMAC_SIZE];
} D3D_OMAC;
```



## <a name="members"></a>Члены

<dl> <dt>

**омак**
</dt> <dd>

Массив байтов, содержащий криптографическое значение MAC сообщения.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                                |
| Header<br/>                   | <dl> <dt>D3d9types. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Видеоструктуры Direct3D](direct3d-video-structures.md)
</dt> </dl>

 

 




