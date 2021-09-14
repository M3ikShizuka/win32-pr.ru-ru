---
title: EDITBOX. Жетлинеиндекс
description: Метод Жетлинеиндекс извлекает индекс символа первого символа в строке с указанным индексом строки.
ms.assetid: 1298227a-d839-44fc-bacb-44c3c968bd94
keywords:
- EDITBOX. жетлинеиндекс проигрыватель Windows Media
topic_type:
- apiref
api_name:
- EDITBOX.getLineIndex
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 5f55027bb7d577b7080ad2f006a5a006e718c2d5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126885240"
---
# <a name="editboxgetlineindex"></a>EDITBOX. Жетлинеиндекс

Метод **жетлинеиндекс** извлекает индекс символа первого символа в строке с указанным индексом строки.

``` syntax
        elementID.getLineIndex(index)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="index"></span><span id="INDEX"></span>*номер*
</dt> <dd>

**Число** (**Long**), содержащее индекс строки, индекс которой необходимо получить.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **число** (**Long**).

## <a name="remarks"></a>Комментарии

Если указанный индекс строки равен 1, то используется строка, содержащая точку вставки.

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

[**EDITBOX. Жетлинефромчар**](editbox-getlinefromchar.md)
</dt> </dl>

 

 





