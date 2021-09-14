---
title: Идентификатор типа безопасности (Чаннелпублишингтипе), элемент
description: Определяет, следует ли включать идентификатор безопасности (SID) участника с каждым событием, записанным в канал.
ms.assetid: 3ce176a3-9e21-4646-8c99-7beb687e6847
keywords:
- Журнал событий элемента идентификатор типа безопасности
topic_type:
- apiref
api_name:
- sidType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 5d65e1ade4ded95b070b45de9462f6aee2c60ac0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127243364"
---
# <a name="sidtype-channelpublishingtype-element"></a>Идентификатор типа безопасности (Чаннелпублишингтипе), элемент

Определяет, следует ли включать идентификатор безопасности (SID) участника с каждым событием, записанным в канал.

``` syntax
<xs:element name="sidType">
    <xs:simpleType>
        <xs:restriction
            base="string"
        >
            <xs:enumeration
                value="None"
             />
            <xs:enumeration
                value="Publishing"
             />
        </xs:restriction>
    </xs:simpleType>
</xs:element>
```

Элемент **идентификатор типа безопасности** определяется сложным типом [**чаннелпублишингтипе**](eventmanifestschema-channelpublishingtype-complextype.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Родительский элемент**
</dt> <dt>

[**Публикация (Чаннелтипе)**](eventmanifestschema-publishing-channeltype-element.md)
</dt> </dl>

 

 





