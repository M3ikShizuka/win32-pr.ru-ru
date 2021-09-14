---
title: Список воспроизведения. Сетселектедстате
description: Метод Сетселектедстате указывает, что в списке воспроизведения выбран индексированный элемент.
ms.assetid: 61770053-733f-40b5-8b1f-92b6975d3ad3
keywords:
- проигрыватель Windows Media списка воспроизведения. сетселектедстате
topic_type:
- apiref
api_name:
- PLAYLIST.setSelectedState
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 09a7bb545330710ae4fe2c39eae4556207061203
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343203"
---
# <a name="playlistsetselectedstate"></a>Список воспроизведения. Сетселектедстате

Метод **сетселектедстате** указывает, что в списке воспроизведения выбран индексированный элемент.

``` syntax
        elementID.setSelectedState(item)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="item"></span><span id="ITEM"></span>*детализирован*
</dt> <dd>

**Число** (**длинное**), указывающее индекс элемента в списке воспроизведения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Вы можете задать для всех элементов выбранное состояние, указав значение 1 в параметре *Item* .

Этот метод был заменен **setSelectedState2**, который поддерживает вложенные списки воспроизведения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент списка воспроизведения**](playlist-element.md)
</dt> <dt>

[**Список воспроизведения. setSelectedState2**](playlist-setselectedstate2.md)
</dt> </dl>

 

 





