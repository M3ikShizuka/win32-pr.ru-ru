---
title: Сообщение LVM_GETSELECTIONMARK (Коммктрл. h)
description: Извлекает метку выделения из элемента управления "представление списка". Это сообщение можно отправить явным образом или использовать \_ макрос Жетселектионмарк ListView.
ms.assetid: 21daf7d7-1217-4608-93f9-c390546f1591
keywords:
- элементы управления Windows сообщений LVM_GETSELECTIONMARK
topic_type:
- apiref
api_name:
- LVM_GETSELECTIONMARK
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 076aff15ff69c4b442c74022ed5a7c02b92a8c52
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054065"
---
# <a name="lvm_getselectionmark-message"></a>\_Сообщение LVM жетселектионмарк

Извлекает метку выделения из элемента управления "представление списка". Это сообщение можно отправить явным образом или использовать макрос [**\_ жетселектионмарк ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_getselectionmark) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает знак выбора, начинающийся с нуля, или значение-1, если нет отметки выделения.

## <a name="remarks"></a>Комментарии

*Отметка выделения* — это индекс элемента, с которого начинается выбор нескольких элементов.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**LVM \_ сетселектионмарк**](lvm-setselectionmark.md)
</dt> </dl>

 

 





