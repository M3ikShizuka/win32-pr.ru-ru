---
title: Сообщение HDM_SETBITMAPMARGIN (Коммктрл. h)
description: Задает ширину поля, заданное в пикселях точечного рисунка в существующем элементе управления "заголовок". Это сообщение можно отправить явным образом или воспользоваться заголовком \_ макроса сетбитмапмаргин.
ms.assetid: 5ac04701-18c8-42d4-9850-fe6eb813672c
keywords:
- элементы управления Windows сообщений HDM_SETBITMAPMARGIN
topic_type:
- apiref
api_name:
- HDM_SETBITMAPMARGIN
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d2a5384151a63918a5828608b0aa8e829df61cad
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054224"
---
# <a name="hdm_setbitmapmargin-message"></a>\_Сообщение СЕТБИТМАПМАРГИН HDM

Задает ширину поля, заданное в пикселях точечного рисунка в существующем элементе управления "заголовок". Это сообщение можно отправить явным образом или воспользоваться [**заголовком макроса \_ сетбитмапмаргин**](/windows/desktop/api/Commctrl/nf-commctrl-header_setbitmapmargin) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Ширина (в пикселях) поля, охватывающего точечный рисунок в существующем элементе управления "заголовок".

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ширину поля точечного рисунка в пикселях. Если поле точечного рисунка не было указано ранее, возвращается значение по умолчанию 3 \* [**жетсистемметрикс**](/windows/desktop/api/winuser/nf-winuser-getsystemmetrics) (*SM \_ ккседже*).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_ЖЕТБИТМАПМАРГИН HDM**](hdm-getbitmapmargin.md)
</dt> </dl>

 

