---
title: Сообщение DTM_CLOSEMONTHCAL (Коммктрл. h)
description: Закрывает элемент управления "Выбор даты и времени" (DTP). Отправляйте это сообщение явным образом или с помощью \_ макроса DateTime клосемонскал.
ms.assetid: f60af77f-ec34-4f3d-9427-cda7ac6083bf
keywords:
- элементы управления Windows сообщений DTM_CLOSEMONTHCAL
topic_type:
- apiref
api_name:
- DTM_CLOSEMONTHCAL
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bd79f33576490196bf29fd51316f8ce3daf4ad4b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127174127"
---
# <a name="dtm_closemonthcal-message"></a>\_Сообщение DTM клосемонскал

Закрывает элемент управления "Выбор даты и времени" (DTP). Отправляйте это сообщение явным образом или с помощью макроса [**DateTime \_ клосемонскал**](/windows/desktop/api/Commctrl/nf-commctrl-datetime_closemonthcal) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ноль.

## <a name="remarks"></a>Remarks

Уничтожает элемент управления и отправляет уведомление [ДТН \_ крупный план](dtn-closeup.md) о том, что элемент управления закрывается (в отличие от раскрывающегося уведомления [ДТН \_ ](dtn-dropdown.md) ) к родителю элемента управления.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[\_раскрывающийся список ДТН](dtn-dropdown.md)
</dt> <dt>

[ДТН \_ крупный план](dtn-closeup.md)
</dt> </dl>

 

 





