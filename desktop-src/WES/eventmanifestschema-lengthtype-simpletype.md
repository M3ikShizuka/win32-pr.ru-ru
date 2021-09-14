---
title: Простой тип Ленгстипе
description: Определяет тип длины, используемый для указания числа байтов или символов в элементе данных переменной длины, например двоичных данных или строки ANSI или Юникод.
ms.assetid: a15e4241-cce3-4f62-bc1c-f70fb1ea5d38
keywords:
- Журнал событий простого типа Ленгстипе
topic_type:
- apiref
api_name:
- LengthType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: dbb0720c2e26fa73056ccffdd17392e93e491c11
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127241087"
---
# <a name="lengthtype-simple-type"></a>Простой тип Ленгстипе

Определяет тип длины, используемый для указания числа байтов или символов в элементе данных переменной длины, например двоичных данных или строки ANSI или Юникод. Значение может быть указано в виде значения xs: Унсигнедшорт или в виде строки, ссылающейся на имя узла элемента данных, который содержит короткое значение без знака.

``` syntax
<xs:simpleType name="LengthType">
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



 

 





