---
title: простой тип UInt32Type (журнал событий Windows)
description: простой тип UInt32Type (журнал событий Windows) — определяет целочисленный тип без знака.
ms.assetid: 11e99c26-3be7-4fac-b3e1-97cb0428a886
keywords:
- Журнал событий простого типа UInt32Type
topic_type:
- apiref
api_name:
- UInt32Type
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 631bb3e8424db8a5d781aaa43df6096730aaa4d6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066771"
---
# <a name="uint32type-simple-type-windows-event-log"></a>простой тип UInt32Type (журнал событий Windows)

Определяет целочисленный тип без знака. Значение может быть указано в виде 4-байтового целого или шестнадцатеричного значения в диапазоне от 0 до 4 294 967 295.

``` syntax
<xs:simpleType name="UInt32Type">
    <xs:union
        memberValues="unsignedInt HexInt32Type"
     />
</xs:simpleType>
```

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





