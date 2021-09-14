---
description: Определяет 4-байтовый шестнадцатеричный тип.
ms.assetid: d0e538c1-f22e-4905-ba73-b670fa7eb174
title: Простой тип HexInt32Type (счетчики производительности)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- kbSyntax
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 2d2392f2240ca9ca61525b27993e16bcab979a97
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127250630"
---
# <a name="hexint32type-simple-type-performance-counters"></a>Простой тип HexInt32Type (счетчики производительности)

Определяет 4-байтовый шестнадцатеричный тип.

``` syntax
<xs:simpleType name="HexInt32Type">
    <xs:restriction
        base="xs:string"
    >
        <xs:pattern
            value="0[xX][0-9A-Fa-f]{1,8}"
         />
    </xs:restriction>
</xs:simpleType>
```

## <a name="patterns"></a>Шаблоны

Простой тип **HexInt32Type** — это **Строка типа xs: String** , которая ограничена следующим шаблоном:

-   `0[xX][0-9A-Fa-f]{1,8}`

    Значение может содержать от одного до восьми шестнадцатеричных символов (например, 0xA или 0xac7bd361).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 




