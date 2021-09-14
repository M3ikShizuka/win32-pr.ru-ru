---
title: Сообщение CB_GETDROPPEDWIDTH (Winuser. h)
description: Возвращает минимально допустимую ширину (в пикселях) поля со списком в \_ раскрывающемся списке или \_ стиле DROPDOWNLIST.
ms.assetid: d7f37a6c-a623-4b15-8ef7-4b64d85c15fa
keywords:
- элементы управления Windows сообщений CB_GETDROPPEDWIDTH
topic_type:
- apiref
api_name:
- CB_GETDROPPEDWIDTH
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 299b360348a6bf7378fdfc9bc9f0959b01366642
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054797"
---
# <a name="cb_getdroppedwidth-message"></a>\_Сообщение ЖЕТДРОППЕДВИДС CB

Возвращает минимально допустимую ширину (в пикселях) поля со списком в [**\_ раскрывающемся**](combo-box-styles.md) списке или стиле [**\_ DROPDOWNLIST**](combo-box-styles.md) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если сообщение прошло удачно, возвращаемое значение будет шириной в пикселях.

Если сообщение не выполняется, возвращается значение CB \_ Err.

## <a name="remarks"></a>Комментарии

По умолчанию минимальная допустимая ширина раскрывающегося списка равна нулю. Ширина списка является либо минимальной допустимой шириной, либо шириной поля со списком, в зависимости от того, какое значение больше.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_СЕТДРОППЕДВИДС CB**](cb-setdroppedwidth.md)
</dt> </dl>

 

 





