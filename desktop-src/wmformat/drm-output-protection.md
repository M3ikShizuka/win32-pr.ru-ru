---
title: Структура DRM_OUTPUT_PROTECTION (Вмдрмсдк. h)
description: '\_Структура защиты выходных данных DRM \_ содержит сведения о технологии защиты выходных данных.'
ms.assetid: e458013d-b77e-4e03-bff9-e3ecfc72ebdb
keywords:
- Формат DRM_OUTPUT_PROTECTION структуры Windows Media
- структура формат мультимедиа Windows
topic_type:
- apiref
api_name:
- DRM_OUTPUT_PROTECTION
api_location:
- Wmdrmsdk.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3a10428d86503e952dc82a7d45bddc11f5dd1286
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127344106"
---
# <a name="drm_output_protection-structure"></a>\_Структура защиты выходных данных DRM \_

Структура **\_ \_ защиты выходных данных DRM** содержит сведения о технологии защиты выходных данных.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct DRM_OUTPUT_PROTECTION {
  GUID guidId;
  BYTE bConfigData;
} ;
```



## <a name="members"></a>Участники

<dl> <dt>

**guidId**
</dt> <dd>

Идентификатор GUID, определяющий технологию защиты выходных данных.

</dd> <dt>

**бконфигдата**
</dt> <dd>

Данные конфигурации для технологии.

</dd> </dl>

## <a name="remarks"></a>Remarks

**DRM \_ Защита \_ аудио \_** и **\_ видео \_ \_ DRM** в инструкциях **typedef** определяется как **\_ \_ Защита выходных данных DRM** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Вмдрмсдк. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Защита вывода DRM, \_ \_ пример**](drm-output-protection-ex.md)
</dt> <dt>

[**Структуры**](drm-structures.md)
</dt> </dl>

 

 





