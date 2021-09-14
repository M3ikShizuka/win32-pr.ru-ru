---
title: Сообщение RB_SETTEXTCOLOR (Коммктрл. h)
description: Задает цвет текста по умолчанию для элемента управления главной панели.
ms.assetid: 85f120bd-39aa-43f8-a794-3bb4f3fe1cd4
keywords:
- элементы управления Windows сообщений RB_SETTEXTCOLOR
topic_type:
- apiref
api_name:
- RB_SETTEXTCOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 68311572927f2e8dac623c697ac366d37d7ab5fb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167263"
---
# <a name="rb_settextcolor-message"></a>\_Сообщение СЕТТЕКСТКОЛОР RB

Задает цвет текста по умолчанию для элемента управления главной панели.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Значение [**COLORREF**](/windows/desktop/gdi/colorref) , представляющее новый цвет текста по умолчанию.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение [**COLORREF**](/windows/desktop/gdi/colorref) , представляющее предыдущий цвет текста по умолчанию.

## <a name="remarks"></a>Remarks

Цвет текста по умолчанию элемента управления главной панели используется для рисования текста в элементе управления "Главная панель" и всех полос, добавленных после отправки этого сообщения. Цвет текста по умолчанию для определенного диапазона можно переопределить при добавлении или изменении диапазона, установив \_ флаг рббим Colors в **фмаск** и установив **клрбакк** в структуре [**ребарбандинфо**](/windows/win32/api/commctrl/ns-commctrl-rebarbandinfoa) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_ЖЕТТЕКСТКОЛОР RB**](rb-gettextcolor.md)
</dt> </dl>

 

