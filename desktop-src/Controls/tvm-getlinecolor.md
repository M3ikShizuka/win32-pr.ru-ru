---
title: Сообщение TVM_GETLINECOLOR (Коммктрл. h)
description: Сообщение TVM \_ жетлинеколор получает текущий цвет линии.
ms.assetid: e74441b3-5d4f-4454-b896-2e96ce649419
keywords:
- элементы управления Windows сообщений TVM_GETLINECOLOR
topic_type:
- apiref
api_name:
- TVM_GETLINECOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 56ed83649795ccbd9b41270272f5a8984ddf257c3f5881a0c0fb69232081974e
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119914004"
---
# <a name="tvm_getlinecolor-message"></a>\_Сообщение TVM жетлинеколор

Сообщение **TVM \_ жетлинеколор** получает текущий цвет линии.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает текущий цвет строки или \_ значение CLR по умолчанию, если ничего не указано.

## <a name="remarks"></a>Remarks

Это сообщение получает только цвета линий. Чтобы получить цвета "+" и "-" внутри кнопок, используйте сообщение [**TVM \_ жеттекстколор**](tvm-gettextcolor.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**TVM \_ сетлинеколор**](tvm-setlinecolor.md)
</dt> </dl>

 

 





