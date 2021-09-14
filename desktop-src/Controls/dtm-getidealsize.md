---
title: Сообщение DTM_GETIDEALSIZE (Коммктрл. h)
description: Возвращает размер, необходимый для вывода элемента управления без усечения. Отправляйте это сообщение явным образом или с помощью \_ макроса DateTime жетидеалсизе.
ms.assetid: 15ec26a1-645b-4a96-af66-1031e1a46c6c
keywords:
- элементы управления Windows сообщений DTM_GETIDEALSIZE
topic_type:
- apiref
api_name:
- DTM_GETIDEALSIZE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a979883f431fea4627f52fe19c3716341e3f2328
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126892352"
---
# <a name="dtm_getidealsize-message"></a>\_Сообщение DTM жетидеалсизе

Возвращает размер, необходимый для вывода элемента управления без усечения. Отправляйте это сообщение явным образом или с помощью макроса [**DateTime \_ жетидеалсизе**](/windows/desktop/api/Commctrl/nf-commctrl-datetime_getidealsize) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется. Должен равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**размера**](/previous-versions//dd145106(v=vs.85)) для получения идеального размера. Вызывающее приложение отвечает за выделение этой структуры.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

