---
title: Сообщение CB_SETTOPINDEX (Winuser. h)
description: Приложение отправляет \_ сообщение СЕТТОПИНДЕКС CB, чтобы убедиться, что конкретный элемент отображается в списке поля со списком.
ms.assetid: vs|controls|~\controls\comboboxes\comboboxreference\comboboxmessages\cb_settopindex.htm
keywords:
- элементы управления Windows сообщений CB_SETTOPINDEX
topic_type:
- apiref
api_name:
- CB_SETTOPINDEX
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0f402cbd16cd61a829a2221600bd3c548829f348
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170091"
---
# <a name="cb_settopindex-message"></a>\_Сообщение СЕТТОПИНДЕКС CB

Приложение отправляет сообщение **\_ сеттопиндекс CB** , чтобы убедиться, что конкретный элемент отображается в списке поля со списком. Система прокручивает содержимое списка таким образом, чтобы указанный элемент появился в верхней части окна списка или был достигнут максимальный диапазон прокрутки.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Указывает отсчитываемый от нуля индекс элемента списка.

</dd> <dt>

*lParam* 
</dt> <dd>

Этот параметр не используется.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если сообщение прошло успешно, возвращаемое значение равно нулю.

Если сообщение не выполняется, возвращается значение CB \_ Err.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_ЖЕТТОПИНДЕКС CB**](cb-gettopindex.md)
</dt> </dl>

 

 





