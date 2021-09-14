---
title: Сообщение TB_SETTOOLTIPS (Коммктрл. h)
description: Связывает элемент управления ToolTip с панелью инструментов.
ms.assetid: a645f1f2-9333-4e25-985a-107cffb9b97f
keywords:
- элементы управления Windows сообщений TB_SETTOOLTIPS
topic_type:
- apiref
api_name:
- TB_SETTOOLTIPS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 781565658d2c362ca32e36736d6e2d80c3641514
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166556"
---
# <a name="tb_settooltips-message"></a>\_Сообщение СЕТТУЛТИПС ТБ

Связывает элемент управления ToolTip с панелью инструментов.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Обработчик для элемента управления ToolTip.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

Все кнопки, добавленные на панель инструментов перед отправкой сообщения **\_ сеттултипс ТБ** , не будут зарегистрированы в элементе управления ToolTip.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





