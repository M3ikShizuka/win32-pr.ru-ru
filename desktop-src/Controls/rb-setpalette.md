---
title: Сообщение RB_SETPALETTE (Коммктрл. h)
description: Задает текущую палитру элемента управления главной панели.
ms.assetid: 85f0726a-21fd-41b3-aa52-6a0a0c1947fa
keywords:
- элементы управления Windows сообщений RB_SETPALETTE
topic_type:
- apiref
api_name:
- RB_SETPALETTE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e7ee47985c05bcd8a857620e7fe501bddf53bdec
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167279"
---
# <a name="rb_setpalette-message"></a>\_Сообщение СЕТПАЛЕТТЕ RB

Задает текущую палитру элемента управления главной панели.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Объект **хпалетте** , указывающий новую палитру, которую будет использовать элемент управления "Главная панель".

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает объект **хпалетте** , указывающий предыдущую палитру элемента управления главной панели.

## <a name="remarks"></a>Remarks

Приложение, отправляющее это сообщение, отвечает за удаление **хпалетте** , переданных в этом сообщении (см. [**DeleteObject**](/windows/desktop/api/wingdi/nf-wingdi-deleteobject)). Элемент управления "Главная панель" не удалит набор **хпалетте** с этим сообщением.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**панель \_ RB**](rb-getpalette.md)
</dt> </dl>

 

