---
title: Сообщение TDM_CLICK_BUTTON (Коммктрл. h)
description: Имитирует действие нажатия кнопки в диалоговом окне задачи.
ms.assetid: cc8a8252-3418-4a28-bfb7-11d6e3fee903
keywords:
- элементы управления Windows сообщений TDM_CLICK_BUTTON
topic_type:
- apiref
api_name:
- TDM_CLICK_BUTTON
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7758385699a0d280f808a21db4c56487c466c716b3ae0236f77130847cea3aa8
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119876174"
---
# <a name="tdm_click_button-message"></a>Сообщение о нажатии \_ \_ кнопки TDM

Имитирует действие нажатия кнопки в диалоговом окне задачи.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* \[ окне\]
</dt> <dd>

Значение **типа int** , указывающее идентификатор кнопки, которую необходимо щелкнуть.

</dd> <dt>

*lParam* \[ окне\]
</dt> <dd>

Должен равняться нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение игнорируется.

## <a name="remarks"></a>Remarks

Идентификатор кнопки, заданный параметром *wParam* , отправляется в функцию обратного вызова [**таскдиалогкаллбаккпрок**](/windows/win32/api/commctrl/nc-commctrl-pftaskdialogcallback) как часть [кнопки ТДН, которая \_ \_ щелкнула](tdn-button-clicked.md) код уведомления. После возврата функции обратного вызова диалоговое окно задачи закрывается, если в \_ функции обратного вызова было возвращено значение S ОК. Если в \_ функции обратного вызова был возвращен параметр S false, диалоговое окно задачи остается активным.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

