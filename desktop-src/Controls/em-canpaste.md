---
title: Сообщение EM_CANPASTE (RichEdit. h)
description: Определяет, может ли элемент управления Rich-Edit вставлять указанный формат буфера обмена.
ms.assetid: 1b858ad8-1312-407b-b12a-c63668ba9f72
keywords:
- элементы управления Windows сообщений EM_CANPASTE
topic_type:
- apiref
api_name:
- EM_CANPASTE
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: aad400b610a033b6f67177da99876a892d294ec8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246886"
---
# <a name="em_canpaste-message"></a>\_Сообщение КАНПАСТЕ EM

Определяет, может ли элемент управления Rich-Edit вставлять указанный формат буфера обмена.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Указывает [форматы буфера обмена](/windows/desktop/dataxchg/clipboard-formats) для попыток. Чтобы использовать любой формат в буфере обмена, присвойте этому параметру значение 0.

</dd> <dt>

*lParam* 
</dt> <dd>

Этот параметр не используется; оно должно быть равно нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если формат буфера обмена может быть вставлен, возвращаемое значение будет ненулевым.

Если формат буфера обмена не может быть вставлен, возвращаемое значение равно нулю.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**SendMessage**](/windows/desktop/api/winuser/nf-winuser-sendmessage)
</dt> </dl>

 

