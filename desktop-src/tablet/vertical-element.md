---
description: Содержит сведения, описывающие вертикальный компонент линий в бланке, который используется в заметке журнала. Используется, например, если в заметке есть линии сетки.
ms.assetid: af6f485e-13df-41bb-b57a-10d8393b83e7
title: Вертикальный элемент
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f6f05ab8a2160dbf6b987177957e8285385fe4db
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362909"
---
# <a name="vertical-element"></a>Вертикальный элемент

Содержит сведения, описывающие вертикальный компонент линий в бланке, который используется в заметке журнала. Используется, например, если в заметке есть линии сетки.

## <a name="definition"></a>Определение

``` syntax
<xs:element name="Vertical" type="VerticalType" minOccurs="0" />
```

## <a name="parent-elements"></a>Родительские элементы

[**линелайаут**](linelayout-element.md)

## <a name="child-elements"></a>Дочерние элементы

Отсутствует.

## <a name="attributes"></a>Атрибуты




| attribute | Тип | Обязательно | Описание | Возможные значения | 
|-----------|------|----------|-------------|-----------------|
| <strong>Стиль</strong> | <a href="linelayoutstyletype-simple-type.md"><strong>Линелайаутстилетипе</strong></a> simpleType | Обязательно | Указывает тип рисуемой линии. | <ul><li>Нет</li><li>Сплошная</li><li>Штрих</li><li>Точки</li><li>DashDot</li><li>DashDotDot</li><li>Double</li></ul> | 
| <strong>Цвет</strong> | <a href="colortype-simple-type.md"><strong>Колортипе</strong></a> simpleType | Необязательно | Цвет элемента. | Шестнадцатеричное значение RGB. Соответствует следующему регулярному выражению: # [0-9a-zA-Z] {6} . Например, #4a79B5.<br /> | 
| <strong>спаЦингбефоре</strong> | <strong>xs:nonNegativeInteger</strong> | Необязательно | Отступ перед элементом. | Любое неотрицательное целое число. | 
| <strong>спаЦингбетвин</strong> | <strong>xs:nonNegativeInteger</strong> | Необязательно | Интервал между этим элементом и окружающими его элементами. | Любое неотрицательное целое число. | 




 

## <a name="element-information"></a>Сведения об элементе



|  Элемент     | Значение                                                         |
|--------------|---------------------------------------------------------------|
| Тип элемента | [**Вертикалтипе**](verticaltype-complex-type.md) complexType |
| Пространство имен    | urn: schemas-microsoft-com: TabletPC: ричинк                    |
| Имя схемы  | Средство чтения журнала                                                |



 

 

 




