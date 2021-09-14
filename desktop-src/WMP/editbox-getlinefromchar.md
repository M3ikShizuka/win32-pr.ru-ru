---
title: EDITBOX. Жетлинефромчар
description: Метод Жетлинефромчар извлекает индекс строки для указанного индекса символов.
ms.assetid: c3a29bdf-ff63-4b6d-90e8-d414dde87f85
keywords:
- EDITBOX. жетлинефромчар проигрыватель Windows Media
topic_type:
- apiref
api_name:
- EDITBOX.getLineFromChar
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 3462ce628da72ca1e55df79e408fc79e0ec8b63a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126885253"
---
# <a name="editboxgetlinefromchar"></a>EDITBOX. Жетлинефромчар

Метод **жетлинефромчар** извлекает индекс строки для указанного индекса символов.

``` syntax
        elementID.getLineFromChar(index)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="index"></span><span id="INDEX"></span>*номер*
</dt> <dd>

**Число** (**Long**), содержащее индекс символа, индекс строки которого необходимо получить.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **число** (**Long**).

## <a name="remarks"></a>Комментарии

Если указанная позиция символа равно 1, этот метод извлекает индекс строки текущей строки.

Этот метод может быть вызван только после того, как элемент управления станет видимым.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media для Windows XP или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**EDITBOX, элемент**](editbox-element.md)
</dt> <dt>

[**EDITBOX. в строке**](editbox-getline.md)
</dt> <dt>

[**EDITBOX. Жетлинеиндекс**](editbox-getlineindex.md)
</dt> </dl>

 

 





