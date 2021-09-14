---
title: EDITBOX. Жетселектионенд
description: Метод Жетселектионенд извлекает конечное расположение выделенного текста в элементе управления EditBox.
ms.assetid: 82a445da-3c50-41b7-8ac8-da6c860056ba
keywords:
- EDITBOX. жетселектионенд проигрыватель Windows Media
topic_type:
- apiref
api_name:
- EDITBOX.getSelectionEnd
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: f27c2974360e7e77becfa67a27b4e96b529ad1e5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126885245"
---
# <a name="editboxgetselectionend"></a>EDITBOX. Жетселектионенд

Метод **жетселектионенд** извлекает конечное расположение выделенного текста в элементе управления EditBox.

``` syntax
        elementID.getSelectionEnd()
```

## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **число** (**Long**).

## <a name="remarks"></a>Комментарии

Если текст не выбран, этот метод возвращает позицию точки вставки.

Если элемент управления является многострочным, этот метод возвращает индекс символа в элементе управления, а не индекс строки.

Этот метод может быть вызван только после того, как элемент управления станет видимым.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media для Windows XP или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**EDITBOX, элемент**](editbox-element.md)
</dt> <dt>

[**EDITBOX. Жетселектионстарт**](editbox-getselectionstart.md)
</dt> <dt>

[**EDITBOX. Реплацеселектион**](editbox-replaceselection.md)
</dt> <dt>

[**EDITBOX. Сетселектион**](editbox-setselection.md)
</dt> </dl>

 

 





