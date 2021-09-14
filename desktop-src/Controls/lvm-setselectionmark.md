---
title: Сообщение LVM_SETSELECTIONMARK (Коммктрл. h)
description: Задает метку выделения в элементе управления "представление списка". Это сообщение можно отправить явным образом или использовать \_ макрос Сетселектионмарк ListView.
ms.assetid: 3218f1b3-b934-4083-aaaa-e10ef1dbb6bd
keywords:
- элементы управления Windows сообщений LVM_SETSELECTIONMARK
topic_type:
- apiref
api_name:
- LVM_SETSELECTIONMARK
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3efc01068f22585061cae5a6f2c5c0c841810f52
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362668"
---
# <a name="lvm_setselectionmark-message"></a>\_Сообщение LVM сетселектионмарк

Задает метку выделения в элементе управления "представление списка". Это сообщение можно отправить явным образом или использовать макрос [**\_ сетселектионмарк ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_setselectionmark) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Отсчитываемый от нуля индекс новой метки выделения. Если задано значение-1, отметка выделения удаляется.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает предыдущую отметку выделения или-1, если Предыдущая метка выбора отсутствует.

## <a name="remarks"></a>Комментарии

*Отметка выделения* — это индекс элемента, с которого начинается выбор нескольких элементов. Это сообщение не влияет на состояние выбора элемента.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**LVM \_ жетселектионмарк**](lvm-getselectionmark.md)
</dt> </dl>

 

 





