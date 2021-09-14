---
title: Сообщение TBM_GETPAGESIZE (Коммктрл. h)
description: Возвращает число логических позиций, на которое ползунок TrackBar перемещается в ответ на ввод с клавиатуры, например клавиши или, или ввод с помощью мыши, например щелчки в канале TrackBar.
ms.assetid: f0c5feac-2723-440e-96c0-dac37b0531ed
keywords:
- элементы управления Windows сообщений TBM_GETPAGESIZE
topic_type:
- apiref
api_name:
- TBM_GETPAGESIZE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ac58c0b935b468cf8af565fba2db67c88418ee4f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166516"
---
# <a name="tbm_getpagesize-message"></a>Сообщение ТБМа \_ pageSize

Возвращает число логических позиций, на которое ползунок TrackBar перемещается в ответ на ввод с клавиатуры, например клавиши или, или ввод с помощью мыши, например щелчки в канале TrackBar. Логическое положение — это целое число, увеличивающееся в диапазоне значений TrackBar от минимума до максимальной позиции ползунка.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает 32-разрядное значение, указывающее размер страницы для TrackBar.

## <a name="remarks"></a>Remarks

Эта линейка также отправляет сообщение [**WM \_ HSCROLL**](wm-hscroll.md) или [**WM \_ VSCROLL**](wm-vscroll.md) с \_ кодами уведомлений ТБ PageUp и ТБ \_ PageDown в родительское окно, когда оно получает ввод с клавиатуры или с помощью мыши для прокрутки страницы.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ТБМ \_ SETPAGESIZE**](tbm-setpagesize.md)
</dt> </dl>

 

 





