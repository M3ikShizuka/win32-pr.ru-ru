---
description: Указывает поставщик Microsoft Media Foundation для обзора, который отслеживает вызовы API Media Foundation.
ms.assetid: 7c9abda9-7968-463c-b4a9-19b54012ef56
title: Элемент mfdetours
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3cd03711c74c21a9a6ff33d2cc2560e4b6d6e0a3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127580326"
---
# <a name="mfdetours-element"></a>Элемент mfdetours

Указывает поставщик Microsoft Media Foundation для обзора, который отслеживает вызовы API Media Foundation.

## <a name="usage"></a>Использование

``` syntax
<mfdetours
  level = "CDATA">
  child elements
</mfdetours>
```

## <a name="attributes"></a>Атрибуты



| attribute            | Тип             | Обязательно       | Описание                             |
|----------------------|------------------|----------------|-----------------------------------------|
| **level**<br/> | CDATA<br/> | Да<br/> | Уровень трассировки.<br/> <br/> |



## <a name="child-elements"></a>Дочерние элементы



| Элемент                               |
|---------------------------------------|
| [**This**](keyword.md)<br/> |



### <a name="child-element-sequence"></a>Последовательность дочерних элементов

``` syntax
keyword+
```

## <a name="parent-elements"></a>Родительские элементы

| Элемент                                   |
|-------------------------------------------|
| [**providers**](providers.md)<br/> |



## <a name="element-information"></a>Сведения об элементе

:::row:::
    :::column:::
        Может быть пустым
    :::column-end:::
    :::column span="2":::
        Нет
    :::column-end:::
:::row-end:::

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Файл конфигурации Мфтраце](mftrace-configuration-file.md)
</dt> </dl>

 

 




