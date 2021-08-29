---
title: LISTBOX. Фонтфаце
description: Атрибут Фонтфаце указывает или получает шрифт для элемента управления "список".
ms.assetid: 15e3180a-6e1e-4654-a0bb-164d66a86a26
keywords:
- проигрыватель Windows Media LISTBOX. фонтфаце
topic_type:
- apiref
api_name:
- LISTBOX.fontFace
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 54cf9eb2f1377a92e83d3bc27f8c9491a50369a317af19d16eb2bde765f70958
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119054702"
---
# <a name="listboxfontface"></a>LISTBOX. Фонтфаце

Атрибут **фонтфаце** указывает или получает шрифт для элемента управления "список".

``` syntax
        elementID.fontFace
```

## <a name="possible-values"></a>Возможные значения

Этот атрибут является **строкой** для чтения и записи.

## <a name="remarks"></a>Remarks

Этот атрибут может быть именем любого допустимого шрифта, доступного в Windows. проигрыватель Windows Media не поддерживает установку шрифтов, поэтому выберите шрифт, который вы будете использовать в предполагаемой системе.

если указанный **фонтфаце** недоступен в системе пользователя, элемент управления "список" по умолчанию имеет значение "системный шрифт Windows". По умолчанию для английских языковых систем используется значение Tahoma. Для международных систем значение по умолчанию загружается из файла ресурсов.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|---------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media для Windows XP или более поздней версии<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Элемент LISTBOX**](listbox-element.md)
</dt> <dt>

[**Список LISTBOX. fontSize**](listbox-fontsize.md)
</dt> <dt>

[**LISTBOX. fontStyle**](listbox-fontstyle.md)
</dt> </dl>

 

 





