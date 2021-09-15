---
title: TEXT. Фонтфаце
description: Атрибут Фонтфаце указывает или получает гарнитуру для элемента управления "текст".
ms.assetid: 3b39e245-139a-4361-b678-0f9e962996b7
keywords:
- проигрыватель Windows Media TEXT. фонтфаце
topic_type:
- apiref
api_name:
- TEXT.fontFace
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 183b25547e456cb90cac4d2137354679e13d8a96
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458875"
---
# <a name="textfontface"></a>TEXT. Фонтфаце

Атрибут **фонтфаце** указывает или получает гарнитуру для элемента управления "текст".

``` syntax
        elementID.fontFace
```

## <a name="possible-values"></a>Возможные значения

Этот атрибут является **строкой** для чтения и записи.

## <a name="remarks"></a>Комментарии

Этот атрибут может быть именем любого допустимого шрифта, доступного в Windows. проигрыватель Windows Media не поддерживает установку шрифтов, поэтому выберите шрифт, который вы будете использовать в предполагаемой системе.

если указанный **фонтфаце** недоступен в системе пользователя, то элемент управления "текст" по умолчанию имеет значение "системный шрифт Windows".

См. атрибут [value](text-value.md) для примера, иллюстрирующий использование атрибутов **текстового** элемента.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**TEXT, элемент**](text-element.md)
</dt> <dt>

[**TEXT. fontSize**](text-fontsize.md)
</dt> </dl>

 

 





