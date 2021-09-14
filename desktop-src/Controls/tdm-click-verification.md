---
title: Сообщение TDM_CLICK_VERIFICATION (Коммктрл. h)
description: Имитирует нажатие флажка проверки диалогового окна задачи, если оно существует.
ms.assetid: 1c6c135e-4e39-4f1a-88f4-5e9f7181a2dd
keywords:
- элементы управления Windows сообщений TDM_CLICK_VERIFICATION
topic_type:
- apiref
api_name:
- TDM_CLICK_VERIFICATION
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: df61676104169e3084e7cde09439c218f2237e60
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166148"
---
# <a name="tdm_click_verification-message"></a>TDM \_ щелкните \_ сообщение о проверке

Имитирует нажатие флажка проверки диалогового окна задачи, если оно существует.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* \[ окне\]
</dt> <dd>

**Значение true** , чтобы установить флажок проверять состояние флажка; **Значение false** , чтобы снять флажок для этого параметра.

</dd> <dt>

*lParam* \[ окне\]
</dt> <dd>

**Значение true** , чтобы установить флажок в фокусе клавиатуры; В противном случае — **значение false** .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение игнорируется.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





