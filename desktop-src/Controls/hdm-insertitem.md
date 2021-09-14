---
title: Сообщение HDM_INSERTITEM (Коммктрл. h)
description: Вставляет новый элемент в элемент управления "заголовок". Это сообщение можно отправить явным образом или воспользоваться заголовком \_ макроса InsertItem.
ms.assetid: aececf32-090d-4cd4-a239-4435a322f72e
keywords:
- элементы управления Windows сообщений HDM_INSERTITEM
topic_type:
- apiref
api_name:
- HDM_INSERTITEM
- HDM_INSERTITEMA
- HDM_INSERTITEMW
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c9cabf86fea79fd437b3e9fb7e32890b3ba1a780
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054238"
---
# <a name="hdm_insertitem-message"></a>\_Сообщение INSERTITEM HDM

Вставляет новый элемент в элемент управления "заголовок". Это сообщение можно отправить явным образом или воспользоваться [**заголовком макроса \_ InsertItem**](/windows/desktop/api/Commctrl/nf-commctrl-header_insertitem) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Индекс элемента, после которого вставляется новый элемент. Новый элемент вставляется в конец элемента управления заголовка, если параметр *wParam* больше или равен числу элементов в элементе управления. Если параметр *wParam* равен нулю, новый элемент вставляется в начало элемента управления заголовка.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**хдитем**](/windows/win32/api/commctrl/ns-commctrl-hditema) , содержащую сведения о новом элементе.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает индекс нового элемента, если он выполнен успешно, или значение-1 в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **Разъем HDM \_ ИНСЕРТИТЕМВ** (Юникод) и **HDM \_ инсертитема** (ANSI)<br/>             |



 

 





