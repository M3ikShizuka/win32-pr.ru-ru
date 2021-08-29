---
title: Сообщение EM_SETWORDBREAKPROCEX (RichEdit. h)
description: Задает расширенную процедуру разбиения по словам для элемента управления расширенного редактирования.
ms.assetid: 2b45f747-ae15-470b-a786-98d8135289da
keywords:
- элементы управления Windows сообщений EM_SETWORDBREAKPROCEX
topic_type:
- apiref
api_name:
- EM_SETWORDBREAKPROCEX
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ecc56e147c52d89b929a4e7065d4daafc184406247d60d522ef2bf4317097faf
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120062844"
---
# <a name="em_setwordbreakprocex-message"></a>\_Сообщение СЕТВОРДБРЕАКПРОЦЕКС EM

Задает расширенную процедуру разбиения по словам для элемента управления расширенного редактирования.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Этот параметр не используется; оно должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на функцию [*едитвордбреакпроцекс*](/windows/desktop/api/Richedit/nc-richedit-editwordbreakprocex) или **значение NULL** для использования процедуры по умолчанию.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение возвращает адрес предыдущей расширенной процедуры разбиения по словам.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

**Ссылки**
</dt> <dt>

[**едитвордбреакпроцекс**](/windows/desktop/api/Richedit/nc-richedit-editwordbreakprocex)
</dt> <dt>

[**EM \_ жетвордбреакпроцекс**](em-getwordbreakprocex.md)
</dt> </dl>

 

 





