---
description: Содержит список поставщиков трассировки для Мфтраце.
ms.assetid: ee483f0a-5a90-4150-ada4-0b63ae312523
title: Элемент providers
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d38a86bf3ca8ffa1ea9e3da20e0244e7abec8513
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127268763"
---
# <a name="providers-element"></a>Элемент providers

Содержит список поставщиков трассировки для [мфтраце](mftrace.md).

## <a name="usage"></a>Использование

``` syntax
<providers>
  child elements
</providers>
```

## <a name="attributes"></a>Атрибуты

Атрибуты отсутствуют.

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                   | Описание                                                                                                      |
|-------------------------------------------|------------------------------------------------------------------------------------------------------------------|
| [**мфдетаурс**](mfdetours.md)<br/> | Указывает поставщик Media Foundation для обзора, который отслеживает вызовы API Media Foundation.<br/> <br/> |
| [**поставщики**](provider.md)<br/>   | Указывает поставщика трассировки (ETW или WPP).<br/> <br/>                                                  |



### <a name="child-element-sequence"></a>Последовательность дочерних элементов

``` syntax
(
  mfdetours?, 
  provider*
)
```

## <a name="parent-elements"></a>Родительские элементы

Нет родительских элементов.

## <a name="element-information"></a>Сведения об элементе

:::row:::
    :::column:::
        Может быть пустым
    :::column-end:::
    :::column span="2":::
        Да
    :::column-end:::
:::row-end:::

## <a name="see-also"></a>См. также

<dl> <dt>

[Файл конфигурации Мфтраце](mftrace-configuration-file.md)
</dt> </dl>

 

 




