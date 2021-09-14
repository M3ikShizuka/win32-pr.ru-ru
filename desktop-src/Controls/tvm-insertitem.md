---
title: Сообщение TVM_INSERTITEM (Коммктрл. h)
description: Вставляет новый элемент в элемент управления представлением в виде дерева. Это сообщение можно отправить явно или с помощью \_ макроса InsertItem TreeView.
ms.assetid: c5e5f88f-6ec8-4b95-89ea-97f6f1fd735e
keywords:
- элементы управления Windows сообщений TVM_INSERTITEM
topic_type:
- apiref
api_name:
- TVM_INSERTITEM
- TVM_INSERTITEMA
- TVM_INSERTITEMW
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 719de4c2391ff924c9f6deb8cb4206cfdb56c3ba
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165687"
---
# <a name="tvm_insertitem-message"></a>\_Сообщение TVM INSERTITEM

Вставляет новый элемент в элемент управления представлением в виде дерева. Это сообщение можно отправить явно или с помощью макроса [**\_ InsertItem TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_insertitem) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**твинсертструкт**](/windows/win32/api/commctrl/ns-commctrl-tvinsertstructa) , указывающую атрибуты элемента представления дерева.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает маркер **хтриитем** для нового элемента, если он успешно, или **значение NULL** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **TVM \_ ИНСЕРТИТЕМВ** (Юникод) и **TVM \_ инсертитема** (ANSI)<br/>             |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[ТВН \_ ендлабеледит](tvn-endlabeledit.md)
</dt> </dl>

 

 





