---
title: Сообщение LVM_FINDITEM (Коммктрл. h)
description: Выполняет поиск элемента представления списка с указанными характеристиками. Это сообщение можно отправить явно или с помощью \_ макроса FindItem в ListView.
ms.assetid: 3b18c8ad-97e6-4f4d-bf89-afb95f925ed1
keywords:
- элементы управления Windows сообщений LVM_FINDITEM
topic_type:
- apiref
api_name:
- LVM_FINDITEM
- LVM_FINDITEMA
- LVM_FINDITEMW
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f1f7dfc19e263a6ab7ad29b5e514fa4e52c1a9ba
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054105"
---
# <a name="lvm_finditem-message"></a>\_Сообщение LVM FINDITEM

Выполняет поиск элемента представления списка с указанными характеристиками. Это сообщение можно отправить явно или с помощью макроса [**\_ FindItem в ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_finditem) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Индекс элемента, с которого начинается поиск, или-1, чтобы начать с начала. Сам указанный элемент исключен из поиска.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**лвфиндинфо**](/windows/win32/api/commctrl/ns-commctrl-lvfindinfoa) , содержащую сведения о том, что искать.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает индекс элемента, если он успешно, или значение-1 в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **LVM \_ ФИНДИТЕМВ** (Юникод) и **LVM \_ финдитема** (ANSI)<br/>                 |



 

 





