---
description: Указывает поставщика трассировки (ETW или WPP) для Мфтраце.
ms.assetid: 692cce3b-ebf5-4a49-8c37-48c8ef6caee7
title: элемент provider
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4213e4d56f8dc2ed73802650e3c7558736cedea8f69fe2148b638fbb92433474
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119034972"
---
# <a name="provider-element"></a>элемент provider

Указывает поставщика трассировки (ETW или WPP) для [мфтраце](mftrace.md).

## <a name="usage"></a>Использование

``` syntax
<provider
  ID = "CDATA"
  level = "CDATA">
  child elements
</provider>
```

## <a name="attributes"></a>Атрибуты



| attribute            | Тип             | Обязательно       | Описание                                              |
|----------------------|------------------|----------------|----------------------------------------------------------|
| **Идентификатор**<br/>    | CDATA<br/> | Да<br/> | Имя или идентификатор GUID поставщика.<br/> <br/> |
| **level**<br/> | CDATA<br/> | Да<br/> | Уровень трассировки.<br/> <br/>                  |



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

 

 




