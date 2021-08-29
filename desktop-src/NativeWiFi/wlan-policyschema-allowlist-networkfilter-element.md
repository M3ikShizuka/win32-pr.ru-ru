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
ms.openlocfilehash: 39eb56800b43bce0696bdfd8fe7dea2f6bbcb3c0b82fcffa39e3144af3c93620
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119800322"
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



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**нетворкфилтер**](wlan-policyschema-networkfilter-wlanpolicy-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**Нетворкфилтер (Вланполици)**](wlan-policyschema-networkfilter-wlanpolicy-element.md)
</dt> </dl>

 

 




