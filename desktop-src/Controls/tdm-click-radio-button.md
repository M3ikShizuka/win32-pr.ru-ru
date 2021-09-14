---
title: Сообщение TDM_CLICK_RADIO_BUTTON (Коммктрл. h)
description: Имитирует действие переключателя щелкните в диалоговом окне задачи.
ms.assetid: ad1616fc-f64d-4575-8bd1-7ce63185d725
keywords:
- элементы управления Windows сообщений TDM_CLICK_RADIO_BUTTON
topic_type:
- apiref
api_name:
- TDM_CLICK_RADIO_BUTTON
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b76d465b1b937359a3d312a401914d497f9c9b22
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166159"
---
# <a name="tdm_click_radio_button-message"></a>TDM \_ щелкните \_ сообщение переключателя \_

Имитирует действие переключателя щелкните в диалоговом окне задачи.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* \[ окне\]
</dt> <dd>

Значение **типа int** , указывающее идентификатор переключателя, который следует щелкнуть.

</dd> <dt>

*lParam* \[ окне\]
</dt> <dd>

Должен равняться нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение игнорируется.

## <a name="remarks"></a>Remarks

Указанный идентификатор переключателя отправляется в функцию обратного вызова [**таскдиалогкаллбаккпрок**](/windows/win32/api/commctrl/nc-commctrl-pftaskdialogcallback) в рамках [ \_ переключателя \_ \_ ТДН](tdn-radio-button-clicked.md) . После возврата функции обратного вызова будет установлен переключатель.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

