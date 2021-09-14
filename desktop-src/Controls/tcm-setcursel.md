---
title: Сообщение TCM_SETCURSEL (Коммктрл. h)
description: Выбирает вкладку в элементе управления "Вкладка". Это сообщение можно отправить явным образом или с помощью \_ макроса табктрл сеткурсел.
ms.assetid: cf709d8c-c522-47c8-8ff3-463dc8e924b5
keywords:
- элементы управления Windows сообщений TCM_SETCURSEL
topic_type:
- apiref
api_name:
- TCM_SETCURSEL
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 90033c5a19b0eb7b73f9ed886e8dad8d1ca4c2ab
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166219"
---
# <a name="tcm_setcursel-message"></a>\_Сообщение СЕТКУРСЕЛ TCM

Выбирает вкладку в элементе управления "Вкладка". Это сообщение можно отправить явным образом или с помощью макроса [**табктрл \_ сеткурсел**](/windows/desktop/api/Commctrl/nf-commctrl-tabctrl_setcursel) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Индекс выбираемой вкладки.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает индекс ранее выбранной вкладки в случае успеха, или-1 в противном случае.

## <a name="remarks"></a>Remarks

Элемент управления "Вкладка" не отправляет код уведомления [ТКН \_ Селчангинг](tcn-selchanging.md) или [ТКН \_ селчанже](tcn-selchange.md) , когда вкладка выбрана с помощью этого сообщения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





