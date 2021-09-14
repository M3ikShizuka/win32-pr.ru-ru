---
title: Сообщение EM_GETIMECOMPTEXT (RichEdit. h)
description: Извлекает текст композиции редактора метода ввода (IME).
ms.assetid: 1516305c-5f87-4ae0-97db-8709c71abacc
keywords:
- элементы управления Windows сообщений EM_GETIMECOMPTEXT
topic_type:
- apiref
api_name:
- EM_GETIMECOMPTEXT
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 834c55d6b5e40de7dcacfeb3e2d0c2e0878a0f3a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126892320"
---
# <a name="em_getimecomptext-message"></a>\_Сообщение ЖЕТИМЕКОМПТЕКСТ EM

Извлекает текст композиции редактора метода ввода (IME).

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Структура [**имекомптекст**](/windows/desktop/api/Richedit/ns-richedit-imecomptext) .

</dd> <dt>

*lParam* 
</dt> <dd>

Буфер, который получает текст композиции. Размер этого буфера содержится в элементе **CB** структуры *wParam* .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

В случае успеха возвращаемое значение представляет собой число символов Юникода, скопированных в буфер. В противном случае он равен нулю.

## <a name="remarks"></a>Комментарии

Это сообщение принимает только строки в Юникоде.

**Предупреждение системы безопасности:** Убедитесь в наличии буфера, достаточного для размера входных данных. В противном случае могут возникнуть проблемы с приложением.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP с пакетом обновления 1 (SP1), \[ только классические приложения\]<br/>                                  |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**имекомптекст**](/windows/desktop/api/Richedit/ns-richedit-imecomptext)
</dt> </dl>

 

 





