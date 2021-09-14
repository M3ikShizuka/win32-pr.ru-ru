---
title: Сообщение EM_GETBIDIOPTIONS (RichEdit. h)
description: Указывает текущее состояние двунаправленных параметров в элементе управления Rich Edit.
ms.assetid: 055581c0-ae59-4601-a3e9-416705af429a
keywords:
- элементы управления Windows сообщений EM_GETBIDIOPTIONS
topic_type:
- apiref
api_name:
- EM_GETBIDIOPTIONS
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7fade63ac94007bedbf58642dc7a9451eb158fc3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054458"
---
# <a name="em_getbidioptions-message"></a>\_Сообщение ЖЕТБИДИОПТИОНС EM

Указывает текущее состояние двунаправленных параметров в элементе управления Rich Edit.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Этот параметр не используется; оно должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Структура [**бидиоптионс**](/windows/desktop/api/Richedit/ns-richedit-bidioptions) , которая получает текущее состояние двунаправленных параметров в элементе управления Rich Edit.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение не возвращает значение.

## <a name="remarks"></a>Комментарии

Это сообщение устанавливает для элементов **вмаск** и **веффектс** значения текущего состояния двунаправленных параметров в элементе управления Rich Edit.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Распространяемые компоненты<br/>          | Расширенное редактирование 3,0<br/>                                                              |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[**бидиоптионс**](/windows/desktop/api/Richedit/ns-richedit-bidioptions)
</dt> <dt>

[**EM \_ сетбидиоптионс**](em-setbidioptions.md)
</dt> </dl>

 

 





