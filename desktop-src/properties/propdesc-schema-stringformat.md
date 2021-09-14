---
description: 'Указывает, как Ипропертидескриптион:: Форматфордисплай должен форматировать значение свойства stringFormat в виде строки.'
ms.assetid: 7c38bc15-be86-4260-b2e4-13afc90de6d7
title: stringFormat
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6eb40ec92ed7b31486062b5cca027eb5257e07af
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127268232"
---
# <a name="stringformat"></a>stringFormat

Указывает, как [**ипропертидескриптион:: форматфордисплай**](/windows/win32/api/propsys/nf-propsys-ipropertydescription-formatfordisplay) должен форматировать значение свойства в виде строки. Это применимо только в том случае <displayInfo displayType="String"> , если. Для каждого элемента [displayInfo](./propdesc-schema-displayinfo.md) должен быть только один элемент [StringFormat]() .

При наличии нескольких элементов используется последний из них. Если элемент [StringFormat]() не указан, к описанию свойства применяются параметры атрибута по умолчанию.

## <a name="syntax"></a>Синтаксис


```
<!-- stringFormat -->
<xs:element name="stringFormat"  minOccurs="0" maxOccurs="1">
    <xs:complexType>
        <xs:attribute name="formatAs">
            <xs:simpleType>
                <xs:restriction base="xs:string">
                    <xs:enumeration value="General"/>
                    <xs:enumeration value="FileName"/>
                    <xs:enumeration value="FilePath"/>
                    <xs:enumeration value="Hyperlink"/>
                </xs:restriction>
            </xs:simpleType>
        </xs:attribute>
    </xs:complexType>
</xs:element>
```



## <a name="element-information"></a>Сведения об элементе



| Родительский элемент                                   | Дочерние элементы |
|--------------------------------------------------|----------------|
| [displayInfo](./propdesc-schema-displayinfo.md) | Нет           |



 

## <a name="attributes"></a>Атрибуты



<table>
<colgroup>
<col  />
<col  />
</colgroup>
<thead>
<tr class="header">
<th>Атрибут</th>
<th>Описание</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>форматас</td>
<td>Общедоступный. Необязательный элемент. Значение по умолчанию — &quot; General &quot; . Допустимы следующие значения. 
<table>
<thead>
<tr class="header">
<th>Значение</th>
<th>Значение</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Общие сведения</td>
<td>По умолчанию. Возвращает значение в виде неформатированной строки.</td>
</tr>
<tr class="even">
<td>FileName</td>
<td>Форматирует значение в виде имени файла. Скрывает расширение в соответствии с параметрами пользователя. Требует, чтобы тип свойства был строковым.</td>
</tr>
<tr class="odd">
<td>FilePath</td>
<td>Форматирует значение как путь к файлу. Скрывает расширение в соответствии с параметрами пользователя. Требует, чтобы тип свойства был строковым.</td>
</tr>
<tr class="even">
<td>Гиперссылка</td>
<td>Форматирует значение как гиперссылку.</td>
</tr>
</tbody>
</table>

<p> </p></td>
</tr>
</tbody>
</table>



 

 

 
