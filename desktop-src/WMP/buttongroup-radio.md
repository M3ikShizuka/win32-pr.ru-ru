---
title: BUTTONGROUP. Radio
description: Атрибут Radio указывает или получает значение, указывающее, состоит ли BUTTONGROUP из переключателей.
ms.assetid: f84479f8-af4f-4ca8-991e-1c2ab39d7110
keywords:
- проигрыватель Windows Media BUTTONGROUP. radio
topic_type:
- apiref
api_name:
- BUTTONGROUP.radio
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4e1765a7756aedcebc2b7b030634d8598a5cd89e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126885325"
---
# <a name="buttongroupradio"></a>BUTTONGROUP. Radio

Атрибут **Radio** указывает или получает значение, указывающее, состоит ли **BUTTONGROUP** из переключателей.

``` syntax
        elementID.radio
```

## <a name="possible-values"></a>Возможные значения

Этот атрибут является **логическим значением** для чтения и записи.



| Значение | Описание                                      |
|-------|--------------------------------------------------|
| Да  | **BUTTONGROUP** имеет вид радио.              |
| false | По умолчанию. **BUTTONGROUP** не является стилем радио. |



 

## <a name="remarks"></a>Комментарии

Если параметру **Radio** присвоено значение true, все элементы **буттонелемент** в **BUTTONGROUP** будут закрепляться, но только одна кнопка будет находиться в неправильном состоянии.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**БУТТОНЕЛЕМЕНТ. Клейкие**](buttonelement-sticky.md)
</dt> <dt>

[**BUTTONGROUP, элемент**](buttongroup-element.md)
</dt> </dl>

 

 





