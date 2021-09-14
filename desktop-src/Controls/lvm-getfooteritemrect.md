---
title: Сообщение LVM_GETFOOTERITEMRECT (Коммктрл. h)
description: Возвращает координаты нижнего колонтитула для указанного элемента в элементе управления "представление списка". Отправьте это сообщение явным образом или с помощью \_ макроса Жетфутеритемрект ListView.
ms.assetid: 4a6055d3-1cc1-4c3d-a5f6-006617ff3bce
keywords:
- элементы управления Windows сообщений LVM_GETFOOTERITEMRECT
topic_type:
- apiref
api_name:
- LVM_GETFOOTERITEMRECT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 142cb92806fa1d58faa0414c10c41bd2815d5b6b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126972126"
---
# <a name="lvm_getfooteritemrect-message"></a>\_Сообщение LVM жетфутеритемрект

Возвращает координаты нижнего колонтитула для указанного элемента в элементе управления "представление списка". Отправьте это сообщение явным образом или с помощью макроса [**\_ жетфутеритемрект ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_getfooteritemrect) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* \[ окне\]
</dt> <dd>

Индекс элемента в элементе управления List-View.

</dd> <dt>

*lParam* \[ в, out\]
</dt> <dd>

Указатель на структуру [**Rect**](/previous-versions//dd162897(v=vs.85)) для получения координат. Вызывающее приложение отвечает за выделение этой структуры. Полученные координаты выражаются как клиентские координаты.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

