---
title: Сообщение TVM_SETLINECOLOR (Коммктрл. h)
description: В \_ сообщении TVM сетлинеколор устанавливается текущий цвет линии.
ms.assetid: c5fc28af-5603-489f-aa6b-73e153f9aebc
keywords:
- элементы управления Windows сообщений TVM_SETLINECOLOR
topic_type:
- apiref
api_name:
- TVM_SETLINECOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7d70340ea0d2339055faa3fb473269f3b244f335
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165620"
---
# <a name="tvm_setlinecolor-message"></a>\_Сообщение TVM сетлинеколор

В сообщении **TVM \_ сетлинеколор** устанавливается текущий цвет линии.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Цвет новой линии. Используйте \_ значение по умолчанию CLR для восстановления системных цветов по умолчанию.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает цвет предыдущей строки.

## <a name="remarks"></a>Remarks

Это сообщение изменяет только цвета линий. Чтобы изменить цвета "+" и "-" внутри кнопок, используйте сообщение [**TVM \_ сеттекстколор**](tvm-settextcolor.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**TVM \_ жетлинеколор**](tvm-getlinecolor.md)
</dt> </dl>

 

 





