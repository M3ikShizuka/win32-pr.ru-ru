---
title: Сообщение TB_HIDEBUTTON (Коммктрл. h)
description: Скрывает или отображает указанную кнопку на панели инструментов.
ms.assetid: 57941a40-279a-426e-baf9-115429c62839
keywords:
- элементы управления Windows сообщений TB_HIDEBUTTON
topic_type:
- apiref
api_name:
- TB_HIDEBUTTON
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 08c5df2f402f1b2de476a3d4748a69a4bb954ff2122855299f49ea1ddba37f7f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119078278"
---
# <a name="tb_hidebutton-message"></a>\_Сообщение ХИДЕБУТТОН ТБ

Скрывает или отображает указанную кнопку на панели инструментов.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Идентификатор команды для скрытия или отображения.

</dd> <dt>

*lParam* 
</dt> <dd>

[**Ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85)) — это **логическое** значение, указывающее, следует ли скрывать или отображать указанную кнопку. Если **значение равно true**, кнопка скрыта. Если задано **значение false**, отображается кнопка.

[**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85)) должен быть равен нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

