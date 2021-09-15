---
title: Список воспроизведения. sortColumn
description: Метод sortColumn сортирует данные в указанном столбце.
ms.assetid: 1563fee8-044a-4cb4-a9c2-11d4533536da
keywords:
- проигрыватель Windows Media списка воспроизведения. sortColumn
topic_type:
- apiref
api_name:
- PLAYLIST.sortColumn
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: f21f0032ee4db4c7af46b5dda814bb11db551330
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570102"
---
# <a name="playlistsortcolumn"></a>Список воспроизведения. sortColumn

Метод **sortColumn** сортирует данные в указанном столбце.

``` syntax
        elementID.sortColumn(column)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="column"></span><span id="COLUMN"></span>*рубрик*
</dt> <dd>

**Число** (**Long**), указывающее индекс столбца для сортировки.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод сортирует указанный столбец так же, как кнопки заголовка столбца в элементе **списка воспроизведения** . Если столбец еще не отсортирован, он сортируется в алфавитно-цифровом порядке. Если сортировка выполнена, ее порядок изменяется на обратный.

Чтобы этот метод работал, атрибуту **алловколумнсортинг** должно быть присвоено значение true.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент списка воспроизведения**](playlist-element.md)
</dt> <dt>

[**Список воспроизведения. Алловколумнсортинг**](playlist-allowcolumnsorting.md)
</dt> </dl>

 

 





