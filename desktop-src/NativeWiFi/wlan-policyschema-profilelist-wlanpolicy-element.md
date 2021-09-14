---
description: Элемент Профилелист (Вланполици) — содержит список профилей, применяемых на уровне домена или компьютера.
ms.assetid: b78cb095-a1da-4b1b-91d3-c5085325be05
title: Профилелист (Вланполици), элемент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- profileList
api_type:
- Schema
api_location: ''
ms.openlocfilehash: 4c7478f38ba7336738325bac6872866cd570288b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127147010"
---
# <a name="profilelist-wlanpolicy-element"></a>Профилелист (Вланполици), элемент

Элемент Профилелист (Вланполици) содержит список профилей, применяемых на уровне домена или компьютера. Этот элемент является необязательным. Если этот элемент имеется, он должен содержать по крайней мере один профиль.

Профили должны основываться на [ \_ схеме профиля WLAN](wlan-profileschema-schema.md)с корневым элементом [**вланпрофиле**](wlan-profileschema-wlanprofile-element.md).

``` syntax
<xs:element name="profileList">
    <xs:complexType>
        <xs:sequence>
            <xs:any
                processContents="lax"
                maxOccurs="unbounded"
                namespace="##other"
             />
        </xs:sequence>
    </xs:complexType>
</xs:element>
```

Элемент **профилелист** определяется элементом [**вланполици**](wlan-policyschema-wlanpolicy-element.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**вланполици**](wlan-policyschema-wlanpolicy-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**вланполици**](wlan-policyschema-wlanpolicy-element.md)
</dt> </dl>

 

 




