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
ms.openlocfilehash: e73e8bd013836767e2a943616407aea9f563fea2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127245446"
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

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista, Windows XP с пакетом обновления 3 (SP3), \[ только классические приложения\]<br/> |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                |
| Распространяемые компоненты<br/>          | API беспроводной локальной сети для Windows XP с пакетом обновления 2 (SP2)<br/>                 |



 

 




