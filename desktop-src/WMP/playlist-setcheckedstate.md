---
title: Список воспроизведения. Сетчеккедстате
description: Метод Сетчеккедстате указывает, что установлен индексированный элемент в списке воспроизведения.
ms.assetid: ce5de21b-6354-485e-b6f7-f4d090c149f7
keywords:
- проигрыватель Windows Media списка воспроизведения. сетчеккедстате
topic_type:
- apiref
api_name:
- PLAYLIST.setCheckedState
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 6a8c86459dcf590b1ff1e884a8aa671dc1bba78a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343218"
---
# <a name="playlistsetcheckedstate"></a>Список воспроизведения. Сетчеккедстате

Метод **сетчеккедстате** указывает, что установлен индексированный элемент в списке воспроизведения.

``` syntax
        elementID.setCheckedState(item)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="item"></span><span id="ITEM"></span>*детализирован*
</dt> <dd>

**Число** (**длинное**), указывающее индекс элемента списка воспроизведения, который должен быть проверен.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **логическое значение**.

## <a name="remarks"></a>Remarks

Можно задать для всех элементов состояние checked, указав значение 1 в параметре *Item* .

Этот метод был заменен **setCheckedState2**, который поддерживает вложенные списки воспроизведения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент списка воспроизведения**](playlist-element.md)
</dt> <dt>

[**Список воспроизведения. setCheckedState2**](playlist-setcheckedstate2.md)
</dt> </dl>

 

 





