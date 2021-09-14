---
title: Сообщение IPM_SETADDRESS (Коммктрл. h)
description: Задает значения адреса для всех четырех полей в элементе управления "IP-адрес".
ms.assetid: 52e72437-3558-4789-844f-5ab5b0b7967c
keywords:
- элементы управления Windows сообщений IPM_SETADDRESS
topic_type:
- apiref
api_name:
- IPM_SETADDRESS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a8e8e4fa69791f93094d24f990ad62207cad33dc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054148"
---
# <a name="ipm_setaddress-message"></a>\_Сообщение IPM сетаддресс

Задает значения адреса для всех четырех полей в элементе управления "IP-адрес".

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Значение **типа DWORD** , содержащее новый адрес. Значение поля 3 содержится в битах от 0 до 7. Значение поля 2 содержится в битах от 8 до 15. Значение поля 1 содержится в битах от 16 до 23. Значение поля 0 содержится в битах с 24 по 31. Для создания сведений об адресе также можно использовать макрос [**макеипаддресс**](/windows/desktop/api/Commctrl/nf-commctrl-makeipaddress) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение не используется.

## <a name="remarks"></a>Комментарии

Это сообщение не создает уведомление [**ИПН \_ фиелдчанжед**](ipn-fieldchanged.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





