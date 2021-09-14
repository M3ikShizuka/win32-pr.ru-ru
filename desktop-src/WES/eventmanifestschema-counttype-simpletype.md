---
title: Простой тип Каунттипе
description: Определяет тип счетчика, который используется для указания количества элементов в массиве.
ms.assetid: 84f819d7-5c42-475b-9144-aaa5e2d215c8
keywords:
- Журнал событий простого типа Каунттипе
topic_type:
- apiref
api_name:
- CountType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 8f91b19df4182f5cff305de0429a308d0c5db234
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967921"
---
# <a name="counttype-simple-type"></a>Простой тип Каунттипе

Определяет тип счетчика, который используется для указания количества элементов в массиве. Значение может быть указано в виде значения xs: Унсигнедшорт или в виде строки, которая ссылается на имя узла элемента данных, содержащего короткое значение унсижед.

``` syntax
<xs:simpleType name="CountType">
    <xs:union
        memberValues="unsignedShort string"
     />
</xs:simpleType>
```

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





