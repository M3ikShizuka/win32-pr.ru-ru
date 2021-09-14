---
title: Сообщение CB_GETCOUNT (Winuser. h)
description: Возвращает количество элементов списка в поле со списком.
ms.assetid: 69667724-5452-4fcc-afc3-0d98d3beedc8
keywords:
- элементы управления Windows сообщений CB_GETCOUNT
topic_type:
- apiref
api_name:
- CB_GETCOUNT
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7900aadf3ba87cc7603a3fe15f4974911c9f9a37
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173963"
---
# <a name="cb_getcount-message"></a>\_Сообщение о ВЫЧИСЛЕ CB

Возвращает количество элементов списка в поле со списком.

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

Возвращаемое значение — это число элементов в списке. Если возникает ошибка, это может быть значение CB \_ Err.

## <a name="remarks"></a>Remarks

Индекс отсчитывается от нуля, поэтому возвращаемое значение Count больше значения индекса последнего элемента.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



 

 





