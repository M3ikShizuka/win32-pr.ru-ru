---
title: THEME. Шоверрордиалог
description: Метод Шоверрордиалог отображает стандартное диалоговое окно ошибки.
ms.assetid: cec9ecfd-6665-4b0a-a09c-49120d557a80
keywords:
- проигрыватель Windows Media THEME. шоверрордиалог
topic_type:
- apiref
api_name:
- THEME.showErrorDialog
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 0cdc1f9df13ec460ce780507e1bde38a2996f915
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168603"
---
# <a name="themeshowerrordialog"></a>THEME. Шоверрордиалог

Метод **шоверрордиалог** отображает стандартное диалоговое окно ошибки.

``` syntax
        theme.showErrorDialog()
```

## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

если **Параметры. енаблиррордиалогс** имеет значение false, этот метод можно использовать для программного вывода диалогового окна об ошибке. Если в очереди ошибок нет ошибок, диалоговое окно ошибки не отображается.

для серии проигрыватель Windows Media 9 или более поздней версии этот метод должен вызываться из обработчика событий error. проигрыватель Windows Media 9 Series или более поздней версии очищает очередь ошибок для обложек после запуска события ошибки.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент THEME**](theme-element.md)
</dt> <dt>

[**Параметры. енаблиррордиалогс**](settings-enableerrordialogs.md)
</dt> </dl>

 

 





