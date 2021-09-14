---
title: Конфигблоб (Еафостконфиг), элемент
description: Используется, когда конфигурация метода находится в двоичном виде двоичного объекта, а не в виде текстовой строки.
ms.assetid: 2820e0b8-2cd1-40e8-ac0c-a62e73ac3847
keywords:
- Элемент Конфигблоб EAPHost
topic_type:
- apiref
api_name:
- ConfigBlob
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: b220c74c6439b4b2cbb0d05a1d540d673e1bd17b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127252895"
---
# <a name="configblob-eaphostconfig-element"></a>Конфигблоб (Еафостконфиг), элемент

Элемент **конфигблоб (еафостконфиг)** используется, когда конфигурация метода находится в двоичном виде ДВОИЧного объекта, а не в виде текстовой строки.

``` syntax
<xs:element name="ConfigBlob"
    type="hexBinary"
 />
```

Элемент **конфигблоб** определяется элементом [**еафостконфиг**](eaphostconfigschema-eaphostconfig-element.md) .

## <a name="remarks"></a>Комментарии

Элементы [**config**](eaphostconfigschema-config-eaphostconfig-element.md) и **конфигблоб** не могут одновременно использоваться одновременно.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**еафостконфиг**](eaphostconfigschema-eaphostconfig-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**еафостконфиг**](eaphostconfigschema-eaphostconfig-element.md)
</dt> <dt>

[EAPHost и схема прежних версий](eaphost-schemas.md)
</dt> <dt>

[Схема еафостконфиг](eaphostconfigschema-schema.md)
</dt> </dl>

 

 





