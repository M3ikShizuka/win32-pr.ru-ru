---
title: Сообщение DTM_GETSYSTEMTIME (Коммктрл. h)
description: Получает выбранное в данный момент время из элемента управления "Выбор даты и времени" (DTP) и помещает его в указанную структуру SYSTEMTIME. Это сообщение можно отправить явным образом или использовать \_ макрос GetSystemtime типа DateTime.
ms.assetid: 81c95187-109c-4b36-98ea-a2e77ce42d9a
keywords:
- элементы управления Windows сообщений DTM_GETSYSTEMTIME
topic_type:
- apiref
api_name:
- DTM_GETSYSTEMTIME
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 00555079a018f0ed2d8c16fb3efdf23fd710656f318f1bb2bd66a167b25ce135
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119877884"
---
# <a name="dtm_getsystemtime-message"></a>\_Сообщение DTM GETSYSTEMTIME

Получает выбранное в данный момент время из элемента управления "Выбор даты и времени" (DTP) и помещает его в указанную структуру [**SYSTEMTIME**](/windows/desktop/api/minwinbase/ns-minwinbase-systemtime) . Это сообщение можно отправить явным образом или использовать макрос [**\_ GetSystemtime типа DateTime**](/windows/desktop/api/Commctrl/nf-commctrl-datetime_getsystemtime) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**SYSTEMTIME**](/windows/desktop/api/minwinbase/ns-minwinbase-systemtime) . Если **DTM \_ GETSYSTEMTIME** возвращает ГДТ \_ допустимое значение, эта структура будет содержать текущее выбранное время. В противном случае он не будет содержать действительные сведения. Этот параметр должен быть допустимым указателем; Он не может иметь **значение NULL**.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ГДТ \_ , допустимое, если сведения о времени были успешно помещены в *lParam*. Возвращает \_ значение ГДТ None, если элементу управления задан стиль [**DTS \_ шовноне**](date-and-time-picker-control-styles.md) , а флажок Control (элемент управления) не установлен. Возвращает \_ ошибку ГДТ при возникновении ошибки.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

