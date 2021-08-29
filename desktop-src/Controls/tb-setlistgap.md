---
title: Сообщение TB_SETLISTGAP (Коммктрл. h)
description: Задает расстояние между кнопками панели инструментов на определенной панели инструментов.
ms.assetid: ca8ba6e4-cf70-41ca-ac61-cd13671d4010
keywords:
- элементы управления Windows сообщений TB_SETLISTGAP
topic_type:
- apiref
api_name:
- TB_SETLISTGAP
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6192a002fcc2aec52c6c294b9eaad3fc55af3bfa3d01a092ae44f5c6d4087559
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119078178"
---
# <a name="tb_setlistgap-message"></a>\_Сообщение СЕТЛИСТГАП ТБ

Задает расстояние между кнопками панели инструментов на определенной панели инструментов.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Зазор (в пикселях) между кнопками на панели инструментов.

</dd> <dt>

*lParam* 
</dt> <dd>

Не обрабатывается.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

Разрыв между кнопками применяется только к окну элемента управления ToolBar, которое получает это сообщение. Получение этого сообщения запускает перерисовку панели инструментов, если панель инструментов видима в данный момент.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





