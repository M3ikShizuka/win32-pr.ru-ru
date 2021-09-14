---
title: Сообщение TVM_SETITEM (Коммктрл. h)
description: В \_ сообщении TVM сетитем задаются некоторые или все атрибуты элемента представления в виде дерева. Это сообщение можно отправить явно или с помощью \_ макроса Сетитем TreeView.
ms.assetid: 28d288bf-a557-4fce-870c-ffa368ece5a9
keywords:
- элементы управления Windows сообщений TVM_SETITEM
topic_type:
- apiref
api_name:
- TVM_SETITEM
- TVM_SETITEMA
- TVM_SETITEMW
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 95750af3aa43a25f0ff4eae5533df5d9aef23537
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165635"
---
# <a name="tvm_setitem-message"></a>\_Сообщение TVM сетитем

В сообщении **TVM \_ сетитем** задаются некоторые или все атрибуты элемента представления в виде дерева. Это сообщение можно отправить явно или с помощью макроса [**\_ сетитем TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_setitem) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**твитем**](/windows/win32/api/commctrl/ns-commctrl-tvitema) , содержащую новые атрибуты элемента. В [версии 4,71](common-control-versions.md) и более поздних вместо нее можно использовать структуру [**твитемекс**](/windows/win32/api/commctrl/ns-commctrl-tvitemexa) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="remarks"></a>Remarks

Член **хитем** структуры [**твитем**](/windows/win32/api/commctrl/ns-commctrl-tvitema) или [**твитемекс**](/windows/win32/api/commctrl/ns-commctrl-tvitemexa) определяет элемент, а элемент **Mask** указывает, какие атрибуты задаются.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **TVM \_ СЕТИТЕМВ** (Юникод) и **TVM \_ сетитема** (ANSI)<br/>                   |



 

 





