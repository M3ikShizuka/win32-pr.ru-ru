---
title: Список воспроизведения. setSelectedState2
description: Метод setSelectedState2 задает выбранное состояние элемента с указанным индексом в элементе списка воспроизведения.
ms.assetid: 990b834a-f7ed-45b8-99e1-3efd7f4447f4
keywords:
- проигрыватель Windows Media списка воспроизведения. setSelectedState2
topic_type:
- apiref
api_name:
- PLAYLIST.setSelectedState2
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: e1a4e317543765fb24755516a0637b16958ad679
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127243139"
---
# <a name="playlistsetselectedstate2"></a>Список воспроизведения. setSelectedState2

Метод **setSelectedState2** задает выбранное состояние элемента с указанным индексом в элементе **списка воспроизведения** .

``` syntax
        elementID.setSelectedState2(item, selected)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="item"></span><span id="ITEM"></span>*детализирован*
</dt> <dd>

**Число** (**длинное**), указывающее индекс элемента в списке воспроизведения.

</dd> <dt>

<span id="selected"></span><span id="SELECTED"></span>*выбрать*
</dt> <dd>

**Логическое значение** , указывающее, должен ли заданный элемент быть выбран (true) или невыбранным (false).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод может работать с вложенными списками воспроизведения и заменять метод **сетселектедстате** , который не может. Вы можете задать для всех элементов запрошенное состояние, указав значение 1 в параметре *Item* .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент списка воспроизведения**](playlist-element.md)
</dt> <dt>

[**Список воспроизведения. Сетселектедстате**](playlist-setselectedstate.md)
</dt> </dl>

 

 





