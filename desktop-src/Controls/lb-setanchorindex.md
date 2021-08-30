---
title: Сообщение LB_SETANCHORINDEX (Winuser. h)
description: Задает элемент привязки \ 8212;, т. е. элемент, из которого начинается выбор нескольких элементов. Множественный выбор охватывает все элементы из привязанного элемента в элемент курсора.
ms.assetid: vs|controls|~\controls\listboxes\listboxreference\listboxmessages\lb_setanchorindex.htm
keywords:
- элементы управления Windows сообщений LB_SETANCHORINDEX
topic_type:
- apiref
api_name:
- LB_SETANCHORINDEX
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 15d8e1eba4168cfd6dd9a7e18a5b82b252c08908e9e49ce7059ed8fdef5ea95d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120085354"
---
# <a name="lb_setanchorindex-message"></a>Сообщение сетанчориндекс балансировки нагрузки \_

Задает элемент привязки, т. е. элемент, из которого начинается выбор нескольких элементов. Множественный выбор охватывает все элементы из привязанного элемента в элемент курсора.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Задает индекс нового элемента привязки.

Windows 95/Windows 98/Windows Millennium Edition (Windows Me): параметр *wParam* ограничен 16-разрядными значениями. Это означает, что списки не могут содержать более 32 767 элементов. Хотя количество элементов ограничено, общий размер элементов в списке в байтах ограничен только доступной памятью.

</dd> <dt>

*lParam* 
</dt> <dd>

Этот параметр не используется.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если сообщение прошло удачно, возвращаемое значение равно нулю.

Если сообщение не выполняется, возвращается значение фунтов \_ Err.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**жетанчориндекс балансировки нагрузки \_**](lb-getanchorindex.md)
</dt> </dl>

 

 





