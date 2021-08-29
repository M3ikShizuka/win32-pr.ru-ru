---
description: Определяет тип, используемый для указания допустимых значений цвета определенных элементов в XML-файле журнала.
ms.assetid: 10a19f28-d0aa-4126-b3f5-fde35fc5fdb0
title: Простой тип Колортипе
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ColorType
api_type:
- Schema
api_location: ''
ms.openlocfilehash: 92b4f8db5626ec34c66c769f86afe1eac9d37940dce0374b1340430d3e62939d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120009084"
---
# <a name="colortype-simple-type"></a>Простой тип Колортипе

Определяет тип, используемый для указания допустимых значений цвета определенных элементов в XML-файле журнала.

``` syntax
<xs:simpleType name="ColorType">
    <xs:restriction
        base="string"
     />
</xs:simpleType>
```

## <a name="remarks"></a>Remarks

Цвет может быть шестнадцатеричным значением RGB в формате \# RRGGBB. Оно должно соответствовать следующему регулярному выражению: \# \[ 0-9a-fA-F \] {6} . Например: " \# 4a79B5".

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                     |



 

 




