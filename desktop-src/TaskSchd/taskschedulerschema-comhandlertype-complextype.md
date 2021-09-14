---
title: Сложный тип Комхандлертипе
description: Определяет дочерние элементы и сведения о последовательности для элемента Комхандлер.
ms.assetid: 688e79f3-8b7e-4892-8119-b0a457ce9c7f
keywords:
- планировщик задач сложного типа Комхандлертипе
topic_type:
- apiref
api_name:
- comHandlerType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: d36a92651fc46c0a1950ecff00fa59fe56e1d758
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064512"
---
# <a name="comhandlertype-complex-type"></a>Сложный тип Комхандлертипе

Определяет дочерние элементы и сведения о последовательности для элемента [**комхандлер**](taskschedulerschema-comhandler-actiongroup-element.md) .

``` syntax
<xs:complexType name="comHandlerType">
    <xs:complexContent>
        <xs:extension
            base="actionBaseType"
        >
            <xs:all>
                <xs:element name="ClassId"
                    type="guidType"
                 />
                <xs:element name="Data"
                    type="dataType"
                    minOccurs="0"
                 />
            </xs:all>
        </xs:extension>
    </xs:complexContent>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                               | Тип                                                         | Описание                                                        |
|-----------------------------------------------------------------------|--------------------------------------------------------------|--------------------------------------------------------------------|
| [**Класса**](taskschedulerschema-classid-comhandlertype-element.md) | [**гуидтипе**](taskschedulerschema-guidtype-simpletype.md)  | Задает идентификатор класса обработчика.<br/>          |
| [**Данные**](taskschedulerschema-data-comhandlertype-element.md)       | [**dataType**](taskschedulerschema-datatype-complextype.md) | Указывает дополнительные данные, связанные с обработчиком. <br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[планировщик задач сложные типы схемы](task-scheduler-schema-complex-types.md)
</dt> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





