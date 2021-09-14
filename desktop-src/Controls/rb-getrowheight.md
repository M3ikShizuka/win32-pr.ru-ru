---
title: Сообщение RB_GETROWHEIGHT (Коммктрл. h)
description: Получает высоту указанной строки в элементе управления "Главная панель".
ms.assetid: 1ff6a32e-b344-4dbc-b4a4-fb13f11a9d8c
keywords:
- элементы управления Windows сообщений RB_GETROWHEIGHT
topic_type:
- apiref
api_name:
- RB_GETROWHEIGHT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 27ce137eef6168d95abfe493a6f22ab66d58460b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167340"
---
# <a name="rb_getrowheight-message"></a>\_Сообщение ЖЕТРОВХЕИГХТ RB

Получает высоту указанной строки в элементе управления "Главная панель".

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Отсчитываемый от нуля индекс диапазона. Будет извлечена высота строки, содержащей указанный диапазон.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение типа **uint** , представляющее высоту строки в пикселях.

## <a name="remarks"></a>Remarks

Чтобы получить количество строк в элементе управления "Главная панель", используйте [**сообщение \_ RB**](rb-getrowcount.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





