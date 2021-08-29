---
title: Сообщение TB_ENABLEBUTTON (Коммктрл. h)
description: Включает или отключает указанную кнопку на панели инструментов.
ms.assetid: d73851ee-f909-4b70-9514-c45cd3a7e999
keywords:
- элементы управления Windows сообщений TB_ENABLEBUTTON
topic_type:
- apiref
api_name:
- TB_ENABLEBUTTON
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9e4edc2fd7c1e088c376772f38c106cf12f41274de0bc5fda6385851c74126e4
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119919104"
---
# <a name="tb_enablebutton-message"></a>\_Сообщение ЕНАБЛЕБУТТОН ТБ

Включает или отключает указанную кнопку на панели инструментов.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Идентификатор команды для включения или отключения.

</dd> <dt>

*lParam* 
</dt> <dd>

[**Ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85)) — это **логическое** значение, указывающее, следует ли включать или отключать указанную кнопку. Если **значение равно true**, кнопка включена. Если задано **значение false**, кнопка отключена.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="remarks"></a>Remarks

Если кнопка включена, ее можно нажать и проверить.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

