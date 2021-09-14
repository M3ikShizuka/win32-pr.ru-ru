---
title: Config (Еафостконфиг), элемент
description: Используется, когда конфигурация метода находится в текстовом формате XML вместо двоичного BLOB-объекта.
ms.assetid: f47bec23-745f-47db-84db-2556beb6a9e9
keywords:
- Элемент конфигурации EAPHost
topic_type:
- apiref
api_name:
- Config
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: a81c90063a57a9d55d8ab6d9c18486315c187f0e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168435"
---
# <a name="config-eaphostconfig-element"></a>Config (Еафостконфиг), элемент

Элемент **config (еафостконфиг)** используется, когда конфигурация метода находится в текстовой XML-форме вместо двоичного BLOB.

``` syntax
<xs:element name="Config"
    type="BaseEapMethodConfig"
 />
```

Элемент **config** определяется элементом [**еафостконфиг**](eaphostconfigschema-eaphostconfig-element.md) .

## <a name="remarks"></a>Remarks

Элементы **config** и [**конфигблоб**](eaphostconfigschema-configblob-eaphostconfig-element.md) не могут одновременно использоваться одновременно.

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

 

 





