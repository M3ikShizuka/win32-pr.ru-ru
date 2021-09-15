---
description: Указывает список беспроводных ЛОКАЛЬНЫХ сетей, к которым может подключаться любой компьютер.
ms.assetid: e24557d8-dedf-4381-bba0-cdb7ea26083b
title: Разрешенных (Нетворкфилтер), элемент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- allowList
api_type:
- Schema
api_location: ''
ms.openlocfilehash: 5488f962a1ba526b34ca2d10144a150d7c1417d4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461668"
---
# <a name="allowlist-networkfilter-element"></a>Разрешенных (Нетворкфилтер), элемент

Элемент разрешенных (Нетворкфилтер) указывает список беспроводных ЛОКАЛЬНЫХ сетей, к которым может подключаться любой компьютер.

``` syntax
<xs:element name="allowList">
    <xs:complexType>
        <xs:sequence>
            <xs:element name="network"
                type="networkItemType"
                maxOccurs="unbounded"
             />
            <xs:any
                processContents="lax"
                minOccurs="0"
                maxOccurs="unbounded"
                namespace="##other"
             />
        </xs:sequence>
    </xs:complexType>
</xs:element>
```

Элемент **разрешенных** определяется элементом [**нетворкфилтер**](wlan-policyschema-networkfilter-wlanpolicy-element.md) .

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                        | Тип                                                                     | Описание                                              |
|----------------------------------------------------------------|--------------------------------------------------------------------------|----------------------------------------------------------|
| [**сети**](wlan-policyschema-network-allowlist-element.md) | [**нетворкитемтипе**](wlan-policyschema-networkitemtype-complextype.md) | Сеть, к которой может подключаться компьютер.<br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**нетворкфилтер**](wlan-policyschema-networkfilter-wlanpolicy-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**Нетворкфилтер (Вланполици)**](wlan-policyschema-networkfilter-wlanpolicy-element.md)
</dt> </dl>

 

 




