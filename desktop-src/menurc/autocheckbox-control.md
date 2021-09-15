---
title: Элемент управления "автофлажок"
description: Определяет элемент управления автоматического флажка.
ms.assetid: 086f5dd3-267f-4ec6-be37-4e9402f7aede
keywords:
- Меню элемента управления "автофлажок" и другие ресурсы
topic_type:
- apiref
api_name:
- AUTOCHECKBOX
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 842bb3ede2b1f96f3e5b343e351e047d112a8403
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460812"
---
# <a name="autocheckbox-control"></a>Элемент управления "автофлажок"

Определяет элемент управления автоматического флажка. Элемент управления является небольшим прямоугольником (флажок), для которого рядом с ним отображается указанный текст (обычно справа). Когда пользователь выбирает элемент управления, элемент управления выделяет прямоугольник и отправляет сообщение родительскому окну.

Инструкцию **автоcheckbox** можно использовать только в теле [**диалогового окна**](dialog-resource.md) или инструкции [**диаложекс**](dialogex-resource.md) .

``` syntax
AUTOCHECKBOX text, id, x, y, width, height [, style [, extended-style]]
```

<dl> <dt>

<span id="style"></span><span id="STYLE"></span>*стиль*
</dt> <dd>

Стили элемента управления. Это значение может быть сочетанием стиля класса кнопки **\_ автофлажок BS** и стилей **\_ группы** **WS \_ TABSTOP** и WS.

Если стиль не указан, используется стиль по умолчанию `BS_AUTOCHECKBOX | WS_TABSTOP` .

</dd> </dl>

Дополнительные сведения об общем синтаксисе инструкции Control см. в разделе [Общие параметры управления](common-control-parameters.md).

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**AUTO3STATE**](auto3state-control.md)
</dt> <dt>

[Стили кнопок](../controls/button-styles.md)
</dt> <dt>

[**Установка**](checkbox-control.md)
</dt> <dt>

[**ЭЛЕМЕНТА**](control-control.md)
</dt> <dt>

[**STATE3**](state3-control.md)
</dt> </dl>

 

 