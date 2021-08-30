---
description: Содержит фон элемента Жаурналдокумент или элемента Жаурналпаже.
ms.assetid: 48527c4e-50fb-4800-ac87-1646234783ba
title: Элемент Background
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3585b8ca37fe86bd1c687601975ea0ad189d5746
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122473900"
---
# <a name="background-element"></a>Элемент Background

Содержит фон элемента [**жаурналдокумент**](journaldocument-element.md) или элемента [**жаурналпаже**](journalpage-element.md) .

## <a name="definition"></a>Определение

``` syntax
<xs:element name="Background" type="BackgroundType" minOccurs="0" />
```

## <a name="parent-elements"></a>Родительские элементы

[**Stationery**](stationery-element.md)

## <a name="child-elements"></a>Дочерние элементы

[**Изображение**](image-element.md)

## <a name="attributes"></a>Атрибуты




| attribute | Тип | Обязательно | Описание | Возможные значения | 
|-----------|------|----------|-------------|-----------------|
| <strong>Стиль</strong> | <strong>xs:string</strong> | Обязательно | Задает стиль фона. | <ul><li>None</li><li>Сплошная</li></ul> | 
| <strong>Цвет</strong> | <a href="colortype-simple-type.md"><strong>Колортипе</strong></a> simpleType | Необязательно | Указывает цвет фона. | См. <a href="colortype-simple-type.md"><strong>колортипе</strong></a> simpleType. | 




 

## <a name="element-information"></a>Сведения об элементе



|                  | Значение                                                             |
|------------------|-------------------------------------------------------------------|
| **Тип элемента** | [**Баккграундтипе**](backgroundtype-complex-type.md) complexType |
| **Пространство имен**    | urn: schemas-microsoft-com: TabletPC: ричинк                        |
| **Имя схемы**  | Средство чтения журнала                                                    |



 

 

 



