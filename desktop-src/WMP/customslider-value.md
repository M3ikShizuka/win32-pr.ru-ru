---
title: КУСТОМСЛИДЕР. Value
description: Атрибут value указывает или получает текущую точку ползунка. | КУСТОМСЛИДЕР. Value
ms.assetid: 29e17f48-1848-458d-9da4-316013b21980
keywords:
- кустомслидер. value проигрыватель Windows Media
topic_type:
- apiref
api_name:
- CUSTOMSLIDER.value
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 89be4edd43fc79c8a8938a3861c982068760bcf3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127258776"
---
# <a name="customslidervalue"></a>КУСТОМСЛИДЕР. Value

Атрибут **value** указывает или получает текущую точку ползунка.

``` syntax
        elementID.value
```

## <a name="possible-values"></a>Возможные значения

Этот атрибут является **числом** для чтения и записи (**float**) со значением по умолчанию, равным атрибуту **min** .

## <a name="remarks"></a>Комментарии

**Значение** должно быть больше или равно **минимальному** и меньше или равно **Max**. Если значение выходит за пределы диапазона, выдается предупреждение и значение не изменяется.

## <a name="examples"></a>Примеры

См. атрибут [поситионимаже](customslider-positionimage.md) для примера, иллюстрирующий использование атрибутов элемента **кустомслидер** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**КУСТОМСЛИДЕР, элемент**](customslider-element.md)
</dt> </dl>

 

 





