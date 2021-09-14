---
title: TEXT. Скроллингделай
description: Атрибут Скроллингделай указывает или получает временную задержку между перемещениями с прокруткой.
ms.assetid: b965fe8f-c809-431f-b8fe-f7c3060068ac
keywords:
- проигрыватель Windows Media TEXT. скроллингделай
topic_type:
- apiref
api_name:
- TEXT.scrollingDelay
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e81259ca84c62327bea67ae70d3f9ec3363450fb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145833"
---
# <a name="textscrollingdelay"></a>TEXT. Скроллингделай

Атрибут **скроллингделай** указывает или получает временную задержку между перемещениями с прокруткой.

``` syntax
        elementID.scrollingDelay
```

## <a name="possible-values"></a>Возможные значения

Этот атрибут является **числом** для чтения и записи (**int**), задающим задержку в миллисекундах. Он имеет минимальное значение 30, а значение по умолчанию — 85. Если указано значение, меньшее минимального значения, используется значение по умолчанию.

## <a name="remarks"></a>Remarks

Если для **прокрутки** задано значение false, **скроллингделай** игнорируется.

См. атрибут [value](text-value.md) для примера, иллюстрирующий использование атрибутов **текстового** элемента.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**TEXT, элемент**](text-element.md)
</dt> <dt>

[**TEXT. Scroll**](text-scrolling.md)
</dt> </dl>

 

 





