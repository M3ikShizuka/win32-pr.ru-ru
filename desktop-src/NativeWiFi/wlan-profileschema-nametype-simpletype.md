---
description: Содержит либо имя, либо описание профиля беспроводной локальной сети.
ms.assetid: cb30d76f-051f-4b90-a0e0-24088a99ca9b
title: Простой тип Наметипе (LAN_policy) (профиль)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- nameType
api_type:
- Schema
api_location: ''
ms.openlocfilehash: 9179efbb52a07983f8d40c271ffc5c0b4ab3eea0c7ddd3a73e1ba790f867143f
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119684004"
---
# <a name="nametype-simple-type-lan_policy-for-profileschema"></a>Простой тип Наметипе (LAN_policy) для профилесчема

Простой тип Наметипе может содержать либо имя, либо описание профиля беспроводной локальной сети. Это строковое значение должно содержать от 1 до 255 символов.

``` syntax
<xs:simpleType name="nameType">
    <xs:restriction
        base="string"
    >
        <xs:minLength
            value="1"
         />
        <xs:maxLength
            value="255"
         />
    </xs:restriction>
</xs:simpleType>
```

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista, Windows XP с пакетом обновления 3 (SP3), \[ только классические приложения\]<br/> |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                |
| Распространяемые компоненты<br/>          | API беспроводной локальной сети для Windows XP с пакетом обновления 2 (SP2)<br/>                 |



 

 




