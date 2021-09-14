---
title: Сообщение SB_SETMINHEIGHT (Коммктрл. h)
description: Задает минимальную высоту области отображения окна состояния.
ms.assetid: 346fe654-f808-4191-9c3d-f9a4def08df1
keywords:
- элементы управления Windows сообщений SB_SETMINHEIGHT
topic_type:
- apiref
api_name:
- SB_SETMINHEIGHT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6bcad3bf0cb4d11567e82aae4ef46a95fefe3890
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167116"
---
# <a name="sb_setminheight-message"></a>\_Сообщение SB сетминхеигхт

Задает минимальную высоту области отображения окна состояния.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Минимальная высота окна в пикселях.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

Минимальная высота — это сумма параметра *wParam* и удвоенная ширина (в пикселях) вертикальной границы окна состояния. Приложение должно отправить сообщение [**\_ размером WM**](/windows/desktop/winmsg/wm-size) в окно состояния, чтобы перерисовать окно. Параметры *wParam* и *lParam* сообщения **\_ размера WM** должны иметь значение 0.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

