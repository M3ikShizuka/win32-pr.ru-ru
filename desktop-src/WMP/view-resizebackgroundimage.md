---
title: VIEW. Ресизебаккграундимаже
description: Атрибут Ресизебаккграундимаже указывает или получает значение, указывающее, можно ли изменить размер фонового изображения.
ms.assetid: d18f3def-777f-4a71-961e-73bae98a4c64
keywords:
- просмотреть. ресизебаккграундимаже проигрыватель Windows Media
topic_type:
- apiref
api_name:
- VIEW.resizeBackgroundImage
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 397929d69cc6ac6ad51c29883898c153218afdca
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567471"
---
# <a name="viewresizebackgroundimage"></a>VIEW. Ресизебаккграундимаже

Атрибут **ресизебаккграундимаже** указывает или получает значение, указывающее, можно ли изменить размер фонового изображения.

``` syntax
        elementID.resizeBackgroundImage
```

## <a name="possible-values"></a>Возможные значения

Этот атрибут является **логическим значением** для чтения и записи.



| Значения | Описание                                      |
|--------|--------------------------------------------------|
| Да   | Размер фонового изображения можно изменить.             |
| false  | По умолчанию. Размер фонового изображения не может быть изменен. |



 

## <a name="remarks"></a>Комментарии

Если задать для этого атрибута значение true, размер фонового изображения изменится в соответствии с текущими значениями атрибутов **Width** и **Height** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**VIEW, элемент**](view-element.md)
</dt> <dt>

[**Просмотр. backgroundImage**](view-backgroundimage.md)
</dt> </dl>

 

 





