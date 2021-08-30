---
title: Сообщение EM_GETTEXTMODE (RichEdit. h)
description: Возвращает текущий текстовый режим и уровень отменяемого элемента управления расширенного редактирования.
ms.assetid: 5c976a82-9c51-4700-9db4-a6b0ed7bb852
keywords:
- элементы управления Windows сообщений EM_GETTEXTMODE
topic_type:
- apiref
api_name:
- EM_GETTEXTMODE
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7cb790a05920cd065e5b8c7fe97bc3d9539ae5ea2b75277f4bfe3c6dabbd8ebe
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120048774"
---
# <a name="em_gettextmode-message"></a>\_Сообщение ЖЕТТЕКСТМОДЕ EM

Возвращает текущий текстовый режим и уровень отменяемого элемента управления расширенного редактирования.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение — это одно или несколько значений из типа перечисления [**TEXTMODE**](/windows/win32/api/richedit/ne-richedit-textmode) . Значения указывают текущий текстовый режим и уровень отмены элемента управления.

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

[**EM \_ сеттекстмоде**](em-settextmode.md)
</dt> <dt>

[**TEXTMODE**](/windows/win32/api/richedit/ne-richedit-textmode)
</dt> </dl>

 

 





