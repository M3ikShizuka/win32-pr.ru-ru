---
description: Содержит набор элементов&\# 8212; Абзац, Инкворд, Drawing, Text, Image или Flag&\# 8212;, которые группируются вместе в заметке журнала.
ms.assetid: 59ee3037-7178-41c8-84d5-d5c68fa2cf9b
title: Граупноде, элемент
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c1dd4258628fbd40c19f8cb1acf3fd0bacbc5557abb967b879dcb78031736288
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120008594"
---
# <a name="groupnode-element"></a>Граупноде, элемент

Содержит набор элементов ([**абзац**](paragraph-element.md), [**инкворд**](inkword-element.md), [**Рисование**](drawing-element.md), [**текст**](text-element.md), [**изображение**](image-element.md)или [**флаг**](flag-element.md)), которые группируются в заметке журнала.

## <a name="definition"></a>Определение

``` syntax
<xs:element name="GroupNode" type="GroupNodeType" />
```

## <a name="parent-elements"></a>Родительские элементы

[**Содержимое**](content-element--journal-reader.md)

## <a name="child-elements"></a>Дочерние элементы

[**Paragraph**](paragraph-element.md)

[**инкворд**](inkword-element.md)

[**Рисование**](drawing-element.md)

[**Полнотекстовым**](text-element.md)

[**Изображение**](docimage-element.md)

[**Флаг**](flag-element.md)

## <a name="attributes"></a>Атрибуты



| attribute  | Тип                      | Обязательно | Описание                                                                             | Возможные значения           |
|------------|---------------------------|----------|-----------------------------------------------------------------------------------------|---------------------------|
| **Слева**   | **xs:integer**            | Обязательно | Расстояние от начала до крайней левой точки в ограничивающем прямоугольнике для элемента. | Любое целое число.              |
| **Top**    | **xs:integer**            | Обязательно | Расстояние от начала до самой верхней точки ограничивающего прямоугольника для элемента.  | Любое целое число.              |
| **Width**  | **xs:nonNegativeInteger** | Обязательно | Ширина ограничивающего прямоугольника для элемента.                                          | Любое неотрицательное целое число. |
| **Height** | **xs:nonNegativeInteger** | Обязательно | Высота ограничивающего прямоугольника для элемента.                                         | Любое неотрицательное целое число. |



 

## <a name="element-information"></a>Сведения об элементе



|  Элемент     | Значение                                                     |
|--------------|-----------------------------------------------------------------|
| Тип элемента | [**Граупнодетипе**](groupnodetype-complex-type.md) complexType |
| Пространство имен    | urn: schemas-microsoft-com: TabletPC: ричинк                      |
| Имя схемы  | Средство чтения журнала                                                  |



 

 

 



