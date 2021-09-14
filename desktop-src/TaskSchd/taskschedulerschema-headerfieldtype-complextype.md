---
title: Сложный тип Хеадерфиелдтипе
description: Определяет элементы, используемые для создания поля заголовка в сообщении электронной почты.
ms.assetid: 66036875-1116-46eb-b2f5-8c8ad8373ab1
keywords:
- планировщик задач сложного типа Хеадерфиелдтипе
topic_type:
- apiref
api_name:
- headerFieldType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 7ddbc0ae22c6baf3fd288cbe2ead19dac506afee
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259296"
---
# <a name="headerfieldtype-complex-type"></a>Сложный тип Хеадерфиелдтипе

Определяет элементы, используемые для создания поля заголовка в сообщении электронной почты.

``` syntax
<xs:complexType name="headerFieldType">
    <xs:all>
        <xs:element name="Name"
            type="nonEmptyString"
         />
        <xs:element name="Value"
            type="string"
         />
    </xs:all>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                            | Тип                                                                    | Описание                                                            |
|--------------------------------------------------------------------|-------------------------------------------------------------------------|------------------------------------------------------------------------|
| [**Безымян**](taskschedulerschema-name-headerfieldtype-element.md)   | [**нонемптистринг**](taskschedulerschema-nonemptystring-simpletype.md) | Задает имя поля заголовка в сообщении электронной почты.<br/> |
| [**Значение**](taskschedulerschema-value-headerfieldtype-element.md) | **строка**                                                              | Задает значение поля заголовка в сообщении электронной почты.<br/>  |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





