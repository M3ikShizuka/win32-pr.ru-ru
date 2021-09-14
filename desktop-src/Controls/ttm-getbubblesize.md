---
title: Сообщение TTM_GETBUBBLESIZE (Коммктрл. h)
description: Возвращает ширину и высоту элемента управления ToolTip.
ms.assetid: 6afb971e-f05d-4b7a-b63d-3672bfcc32dc
keywords:
- элементы управления Windows сообщений TTM_GETBUBBLESIZE
topic_type:
- apiref
api_name:
- TTM_GETBUBBLESIZE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 48b48bda0f795473cb48303e88bbf3c1c35df7cd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165931"
---
# <a name="ttm_getbubblesize-message"></a>\_Сообщение ТТМ жетбубблесизе

Возвращает ширину и высоту элемента управления ToolTip.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**тулинфо**](/windows/win32/api/commctrl/ns-commctrl-tttoolinfoa) ToolTip.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ширину подсказки в нижнем слове и высоту в высоком слове в случае успеха. В противном случае возвращается **значение false**.

## <a name="remarks"></a>Remarks

Если \_ Флаги TTF Track и TTF \_ заданы в элементе **Уфлагс** структуры подсказки [**тулинфо**](/windows/win32/api/commctrl/ns-commctrl-tttoolinfoa) , это сообщение можно использовать для точного размещения подсказки.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





