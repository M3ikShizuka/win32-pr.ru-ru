---
description: Это сочетание РТЛРО порядка чтения справа налево, атрибуты Ригхталигнед и Лефтскролл.
ms.assetid: 4eaec16f-ee1c-437b-8b76-7ebbdc4e2f71
title: Атрибут управления BiDi
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d5fd152bbff384961a51350d31759b35ea2b0b4444cac20c78df3dbc7af13bfd
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120045264"
---
# <a name="bidi-control-attribute"></a>Атрибут управления BiDi

Это сочетание [ртлро](rtlro-control-attribute.md)порядка чтения справа налево, атрибуты [ригхталигнед](rightaligned-control-attribute.md)и [лефтскролл](leftscroll-control-attribute.md) .

## <a name="valid-controls"></a>Допустимые элементы управления

[скроллаблетекст](scrollabletext-control.md)

 

[волумекостлист](volumecostlist-control.md)

 

[ComboBox](combobox-control.md)

 

[директорилист](directorylist-control.md)

 

[директорикомбо](directorycombo-control.md)

 

[Правка](edit-control.md)

 

[ListBox](listbox-control.md)

 

[ListView](listview-control.md)

 

[селектионтри](selectiontree-control.md)

 

[волумеселекткомбо](volumeselectcombo-control.md)

## <a name="value"></a>Значение



| Decimal | Шестнадцатеричный | Константа                       |
|---------|-------------|--------------------------------|
| 224     | 0x000000E0  | **мсидбконтролаттрибутесбиди** |



 

## <a name="remarks"></a>Remarks

Чтобы задать этот атрибут для элемента управления, включите двунаправленный бит в столбец Attributes записи элемента управления в [таблице Control](control-table.md).

См. раздел [атрибуты элементов управления](control-attributes.md) и элемент управления, которые необходимо создать в элементах [управления](controls.md).

 

 



