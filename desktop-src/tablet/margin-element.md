---
description: Определяет линии полей, нарисованные на странице.
ms.assetid: c3047706-affd-4feb-9d48-cfb4c7dd6fa0
title: Элемент Margin
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 78c264c2470d070353d1fd19340a161cf765bc05
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127579422"
---
# <a name="margin-element"></a>Элемент Margin

Определяет линии полей, нарисованные на странице.

## <a name="definition"></a>Определение

``` syntax
<xs:complexType name="MarginType">
   <xs:attribute name="Style" use="required" type="LineLayoutStyleType" />
   <xs:attribute name="Color" type="ColorType" />
   <xs:attribute name="Type" type="MarginTypeType" />
   <xs:attribute name="Spacing" type="xs:positiveInteger" />
</xs:complexType>
```

## <a name="parent-elements"></a>Родительские элементы

Отсутствует.

## <a name="child-elements"></a>Дочерние элементы

Нет..

## <a name="attributes"></a>Атрибуты




| attribute | Тип | Обязательно | Описание | Возможные значения | 
|-----------|------|----------|-------------|-----------------|
| <strong>Стиль</strong> | <a href="linelayoutstyletype-simple-type.md"><strong>Линелайаутстилетипе</strong></a> simpleType | Обязательно | Указывает тип рисуемой линии. | <ul><li>Нет</li><li>Сплошная</li><li>Штрих</li><li>Точки</li><li>DashDot</li><li>DashDotDot</li><li>Double</li></ul> | 
| <strong>Цвет</strong> | <a href="colortype-simple-type.md"><strong>Колортипе</strong></a> simpleType | Необязательно | Цвет элемента. | Шестнадцатеричное значение RGB. Соответствует следующему регулярному выражению: # [0-9a-zA-Z] {6} . Например, #4a79B5.<br /> | 
| <strong>Тип</strong> | <a href="margintypetype-simple-type.md"><strong>Маргинтипетипе</strong></a> simpleType | Необязательный | Показывает левое или правое поле. | <ul><li>Левый</li><li>Правый</li></ul> | 
| <strong>Интервал</strong> | <strong>xs:nonNegativeInteger</strong> | Необязательный | Интервал между границами страницы и поля. | Любое неотрицательное целое число. | 




 

## <a name="element-information"></a>Сведения об элементе



|  Элемент     | Значение                                                     |
|--------------|-----------------------------------------------------------|
| Тип элемента | [**Маргинтипе**](margintype-complex-type.md) complexType |
| Пространство имен    | urn: schemas-microsoft-com: TabletPC: ричинк                |
| Имя схемы  | Средство чтения журнала                                            |



 

 

 




