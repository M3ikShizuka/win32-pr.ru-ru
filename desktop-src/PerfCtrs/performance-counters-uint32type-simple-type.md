---
description: Простой тип UInt32Type (счетчики производительности) — определяет целочисленный тип без знака.
ms.assetid: 48df484d-d663-42fa-aaec-51c463bb5350
title: Простой тип UInt32Type (счетчики производительности)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- kbSyntax
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 32f8a4bbf00f569ba98dfc031f62717b1afc8734
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127169148"
---
# <a name="uint32type-simple-type-performance-counters"></a>Простой тип UInt32Type (счетчики производительности)

Определяет целочисленный тип без знака.

``` syntax
<xs:simpleType name="UInt32Type">
    <xs:union
        memberValues="xs:unsignedInt man:HexInt32Type"
     />
</xs:simpleType>
```

## <a name="remarks"></a>Remarks

Значение можно указать в виде 4-байтового целого или шестнадцатеричного значения в диапазоне от 0 до 4 294 967 295.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 




