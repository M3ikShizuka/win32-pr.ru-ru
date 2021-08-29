---
title: Структура DRM_AUDIO_OUTPUT_PROTECTION_IDS_EX (Вмдрмсдк. h)
description: '\_ \_ \_ Структура ИД защиты звука в \_ DRM \_ содержит список идентификаторов защиты звука. Эта структура расширяет \_ \_ \_ идентификаторы защиты звука DRM \_ , добавляя номер версии.'
ms.assetid: e650ddeb-5e41-4ff8-b872-40c85ab519c1
keywords:
- Формат DRM_AUDIO_OUTPUT_PROTECTION_IDS_EX структуры Windows Media
- структура формат мультимедиа Windows
topic_type:
- apiref
api_name:
- DRM_AUDIO_OUTPUT_PROTECTION_IDS_EX
api_location:
- Wmdrmsdk.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2f08489b15efbfae594138185202db0b5b8472570c8e67a6aa71904236c9b6ba
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119705664"
---
# <a name="drm_audio_output_protection_ids_ex-structure"></a>\_ \_ \_ Идентификаторы защиты аудио вывода DRM \_ \_ Структура ex

Структура **\_ \_ \_ \_ \_ ИД защиты звука в DRM** содержит список идентификаторов защиты звука. Эта структура расширяет **\_ \_ \_ \_ идентификаторы защиты звука DRM** , добавляя номер версии.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct DRM_AUDIO_OUTPUT_PROTECTION_IDS_EX {
  DWORD                          dwVersion;
  WORD                           cEntries;
  DRM_AUDIO_OUTPUT_PROTECTION_EX *rgAop;
} ;
```



## <a name="members"></a>Члены

<dl> <dt>

**двверсион**
</dt> <dd>

Номер версии.

</dd> <dt>

**центриес**
</dt> <dd>

Число записей в массиве **ргаоп** .

</dd> <dt>

**ргаоп**
</dt> <dd>

Массив структур **для \_ \_ \_ защиты \_ звука DRM** . **DRM \_ \_Защита звука \_ , \_ например** , представляет собой тип, определенный как [**\_ \_ Защита \_ выходных данных DRM**](drm-output-protection-ex.md), например.

</dd> </dl>

## <a name="remarks"></a>Remarks

Отсутствует.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Вмдрмсдк. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_ \_ \_ идентификаторы защиты звука в DRM \_**](drm-audio-output-protection-ids.md)
</dt> <dt>

[**\_ \_ \_ идентификаторы защиты вывода видео DRM \_ \_ ex**](drm-video-output-protection-ids-ex.md)
</dt> <dt>

[**Структуры**](drm-structures.md)
</dt> </dl>

 

 





