---
title: Сообщение TCM_SETITEMSIZE (Коммктрл. h)
description: Задает ширину и высоту вкладок в элементе управления вкладки с фиксированной шириной или владельцем. Это сообщение можно отправить явным образом или с помощью \_ макроса табктрл сетитемсизе.
ms.assetid: 3935d686-f8bc-41fb-b025-04120cf03f02
keywords:
- элементы управления Windows сообщений TCM_SETITEMSIZE
topic_type:
- apiref
api_name:
- TCM_SETITEMSIZE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e306af3f6462507a181de91104169c5ac7d6ce14
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166203"
---
# <a name="tcm_setitemsize-message"></a>\_Сообщение СЕТИТЕМСИЗЕ TCM

Задает ширину и высоту вкладок в элементе управления вкладки с фиксированной шириной или владельцем. Это сообщение можно отправить явным образом или с помощью макроса [**табктрл \_ сетитемсизе**](/windows/desktop/api/Commctrl/nf-commctrl-tabctrl_setitemsize) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

[**Ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85)) — это значение **типа int** , указывающее новую ширину в пикселях. [**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85)) — это значение **типа int** , указывающее новую высоту в пикселях.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает старую ширину и высоту. Ширина находится в [**ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85)) возвращаемого значения, а высота — в [**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85)).

## <a name="remarks"></a>Remarks

Если для ширины задано значение меньше ширины изображения, установленного параметром [**ImageList \_ CREATE**](/windows/desktop/api/Commctrl/nf-commctrl-imagelist_create), ширина вкладки устанавливается равным наименьшему значению, превышающему ширину изображения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

