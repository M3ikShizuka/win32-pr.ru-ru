---
title: Сообщение EM_EXGETSEL (RichEdit. h)
description: Получает позиции начального и конечного символов выделения в элементе управления Rich Edit.
ms.assetid: 60fcf13e-6c45-4f4e-9b54-70f0985122fb
keywords:
- элементы управления Windows сообщений EM_EXGETSEL
topic_type:
- apiref
api_name:
- EM_EXGETSEL
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: eec9656c4d94dbb8d9a92e90ce689f356bb7916151099d7d82ae8b3e3b3ccd5f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119915824"
---
# <a name="em_exgetsel-message"></a>\_Сообщение ЕКСЖЕТСЕЛ EM

Получает позиции начального и конечного символов выделения в элементе управления Rich Edit.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Этот параметр не используется; оно должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Структура [**чарранже**](/windows/desktop/api/Richedit/ns-richedit-charrange) , которая получает диапазон выбора.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение не возвращает значение.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**чарранже**](/windows/desktop/api/Richedit/ns-richedit-charrange)
</dt> </dl>

 

 





