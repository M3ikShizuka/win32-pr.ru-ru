---
title: Сообщение BM_SETDONTCLICK (Winuser. h)
description: Устанавливает флаг на переключателе, который управляет созданием млрд ДОЛЛных \_ сообщений, когда кнопка получает фокус.
ms.assetid: 91d98bce-abea-4afc-a995-0f426ba7a518
keywords:
- элементы управления Windows сообщений BM_SETDONTCLICK
topic_type:
- apiref
api_name:
- BM_SETDONTCLICK
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4a118b0e9ed3e1ea797cdd0b690aee0fe3c4cc067b72990d884fdd121fcb80c5
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119921244"
---
# <a name="bm_setdontclick-message"></a>\_Сообщение BM сетдонткликк

Устанавливает флаг на переключателе, который управляет созданием [млрд доллных сообщений \_ ](bn-clicked.md) , когда кнопка получает фокус.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* \[ окне\]
</dt> <dd>

**Логическое** значение, указывающее состояние. **Значение true** , чтобы установить флаг; в противном случае — **значение false**.

</dd> <dt>

*lParam* 
</dt> <dd>

Не используется. Должен равняться нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



 

 





