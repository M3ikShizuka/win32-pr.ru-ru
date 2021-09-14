---
title: EDITBOX. в строке
description: Метод GetText извлекает текст для строки с указанным индексом.
ms.assetid: a692c32b-86b9-419e-a3a5-464687be04da
keywords:
- проигрыватель Windows Media EDITBOX./line
topic_type:
- apiref
api_name:
- EDITBOX.getLine
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 3b0b9a15f9eff8c2612e7a242a205c1d9411a60c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127241033"
---
# <a name="editboxgetline"></a>EDITBOX. в строке

Метод **gettext** извлекает текст для строки с указанным индексом.

``` syntax
        elementID.getLine(index)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="index"></span><span id="INDEX"></span>*номер*
</dt> <dd>

**Число** (**Long**), содержащее индекс строки для извлечения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **строку**.

## <a name="remarks"></a>Комментарии

Если индекс является недопустимым, возвращается пустая строка. Этот метод может быть вызван только после того, как элемент управления станет видимым.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media для Windows XP или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**EDITBOX, элемент**](editbox-element.md)
</dt> <dt>

[**EDITBOX. Жетлинефромчар**](editbox-getlinefromchar.md)
</dt> <dt>

[**EDITBOX. Жетлинеиндекс**](editbox-getlineindex.md)
</dt> </dl>

 

 





