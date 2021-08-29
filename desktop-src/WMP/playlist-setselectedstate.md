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
ms.openlocfilehash: 1ba35f2030f4b2fb6e9acfde1a8310e6c9f1dac98b8ba8aa65d56cce206c8e00
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119862244"
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

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Элемент списка воспроизведения**](playlist-element.md)
</dt> <dt>

[**Список воспроизведения. setSelectedState2**](playlist-setselectedstate2.md)
</dt> </dl>

 

 





