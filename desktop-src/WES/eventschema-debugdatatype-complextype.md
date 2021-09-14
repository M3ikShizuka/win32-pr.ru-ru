---
title: Сложный тип Дебугдататипе
description: определяет данные, которые могут быть зарегистрированы для Windows событий препроцессора (WPP) трассировки программного обеспечения.
ms.assetid: 75638e0f-7a26-473e-a0c4-bd8972ac171f
keywords:
- Журнал событий сложных типов Дебугдататипе
topic_type:
- apiref
api_name:
- DebugDataType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: c190d3b2b0e870ac249fed03485828685d5dc770
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127374385"
---
# <a name="debugdatatype-complex-type"></a>Сложный тип Дебугдататипе

определяет данные, которые могут быть зарегистрированы для Windows событий препроцессора (WPP) трассировки программного обеспечения.

``` syntax
<xs:complexType name="DebugDataType">
    <xs:sequence>
        <xs:element name="SequenceNumber"
            type="unsignedInt"
            minOccurs="0"
         />
        <xs:element name="FlagsName"
            type="string"
            minOccurs="0"
         />
        <xs:element name="LevelName"
            type="string"
            minOccurs="0"
         />
        <xs:element name="Component"
            type="string"
         />
        <xs:element name="SubComponent"
            type="string"
            minOccurs="0"
         />
        <xs:element name="FileLine"
            type="string"
            minOccurs="0"
         />
        <xs:element name="Function"
            type="unsignedInt"
            minOccurs="0"
         />
        <xs:element name="Message"
            type="string"
         />
        <xs:any
            minOccurs="0"
            maxOccurs="unbounded"
            processContents="lax"
            namespace="##other"
         />
    </xs:sequence>
    <xs:anyAttribute
        processContents="lax"
        namespace="##other"
     />
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                    | Тип        | Описание                                                                                                        |
|----------------------------------------------------------------------------|-------------|--------------------------------------------------------------------------------------------------------------------|
| [**Компонент**](eventschema-component-debugdatatype-element.md)           | строка      | Имя компонента, который записал в журнал сообщение трассировки.<br/>                                                |
| [**филелине**](eventschema-fileline-debugdatatype-element.md)             | строка      | Имя исходного файла и строка в исходном файле, которая записала в журнал сообщение трассировки.<br/>          |
| [**флагснаме**](eventschema-flagname-debugdatatype-element.md)            | строка      | Значение флага, передаваемое поставщику при его включении.<br/>                                              |
| [**Функция**](eventschema-function-debugdatatype-element.md)             | unsignedInt | Имя функции, которая зарегистрировала сообщение трассировки.<br/>                                                 |
| [**LevelName**](eventschema-levelname-debugdatatype-element.md)           | строка      | Значение уровня, передаваемое поставщику при его включении.<br/>                                             |
| [**Сообщение**](eventschema-message-debugdatatype-element.md)               | строка      | Строка сообщения. XML-код содержит этот элемент, если в событии WPP указано поле Форматтедстринг.<br/> |
| [**SequenceNumber**](eventschema-sequencenumber-debugdatatype-element.md) | unsignedInt | Локальный или глобальный порядковый номер сообщения трассировки.<br/>                                               |
| [**Вспомогательный компонент**](eventschema-subcomponent-debugdatatype-element.md)     | строка      | Имя подкомпонента, который записал в журнал сообщение трассировки.<br/>                                             |



## <a name="remarks"></a>Remarks

Элементы включаются, только если поставщик установил \_ \_ для переменной среды префикс формата% Trace%, чтобы включить их. Дополнительные сведения об этих элементах см. в разделе префикс сообщения трассировки.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





