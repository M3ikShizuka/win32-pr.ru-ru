---
description: '&lt;Элемент Property &gt; указывает свойство, используемое библиотекой. Эти свойства относятся к библиотеке, поэтому нет предопределенного набора имен свойств для использования. Этот элемент является необязательным и не имеет дочерних элементов.'
ms.assetid: 8BF6EC7A-A87E-45fe-A8F0-4B49594E9E7B
title: Элемент Property (схема библиотеки)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f2c08577e6f2e3310f3f1966737edb7e9bf31de7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574518"
---
# <a name="property-element-library-schema"></a>Элемент Property (схема библиотеки)

&lt;Элемент Property &gt; указывает свойство, используемое библиотекой. Эти свойства относятся к библиотеке, поэтому нет предопределенного набора имен свойств для использования. Этот элемент является необязательным и не имеет дочерних элементов.

## <a name="syntax"></a>Синтаксис

``` syntax
<!-- property -->
<xs:element name="property" minOccurs="0" maxOccurs="unbounded">
    <xs:complexType>
        <xs:complexContent>
            <xs:extension base="xs:anyType">
                <xs:attribute name="name" type="canonical-name" use="required"/>
                    <xs:simpleType name="canonical-name">
                        <xs:restriction base="xs:string">
                            <xs:maxLength value="63"/>
                            <xs:pattern value="[0-9A-Za-z.]*"/>
                        </xs:restriction>
                    </xs:simpleType>
                <xs:attribute name="type"/>
            </xs:extension>
        </xs:complexContent>
    </xs:complexType>
</xs:element>
```

## <a name="element-information"></a>Сведения об элементе



| Родительский элемент                                                             | Дочерние элементы |
|----------------------------------------------------------------------------|----------------|
| [Элемент Пропертисторе (схема библиотеки)](schema-library-propertystore.md) | Нет           |



 

## <a name="attributes"></a>Атрибуты




| Атрибут | Описание | Значения | 
|-----------|-------------|--------|
| name | Общедоступный. Обязательный элемент. Отображаемое имя свойства. | 
| тип | Общедоступный. Обязательный элемент. Тип свойства. | <ul><li>Any: по умолчанию. Значение не будет приведено подсистемой свойств. VT_NULL будет возвращено функцией Жетпропертитипе.</li><li>NULL: значение для этого свойства отсутствует. VT_NULL будет возвращено функцией Жетпропертитипе.</li><li>Строка: значение должно быть VT_LPWSTR.</li><li>Boolean: значение должно быть VT_BOOL.</li><li>Byte: значение должно быть VT_UI1.</li><li>Buffer: значение должно быть VT_UI1 | VT_VECTOR буфер байтов.</li><li>Int16: значение должно быть VT_I2.</li><li>UInt16: значение должно быть VT_UI2.</li><li>Int32: значение должно быть VT_I4.</li><li>UInt32: значение должно быть VT_UI4.</li><li>Int64: значение должно быть VT_I8.</li><li>UInt64: значение должно быть VT_UI8.</li><li>Double: значение должно быть VT_R8.</li><li>DateTime: значение должно быть VT_FILETIME.</li><li>GUID: значение должно быть VT_CLSID.</li><li>BLOB-объект. значение должно быть VT_BLOB.</li><li>Объект: значение должно быть VT_UNKNOWN.</li><li>Stream: значение должно быть VT_STREAM.</li><li>Буфер обмена. значение должно быть VT_CF.</li></ul> | 




 

## <a name="remarks"></a>Комментарии

требования для &lt; элемента канонического имени &gt; соответствуют требованиям для Windows поиска и системы свойств Windows. Строка должна иметь тип канонического типа.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Схема описания библиотеки](library-schema-entry.md)
</dt> <dt>

[Схемы свойств](../properties/building-property-handlers-property-schemas.md)
</dt> <dt>

[Схема описания соединителя поиска](../search/search-sconn-desc-schema-entry.md)
</dt> </dl>

 

 
