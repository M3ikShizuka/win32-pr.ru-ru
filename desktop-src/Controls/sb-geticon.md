---
title: Сообщение SB_GETICON (Коммктрл. h)
description: Возвращает значок для части в строке состояния.
ms.assetid: f99508e3-afa8-48fd-b87a-fce41c4410ff
keywords:
- элементы управления Windows сообщений SB_GETICON
topic_type:
- apiref
api_name:
- SB_GETICON
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ab86809df54d796b8e83f05f2a2b9041450ce2fc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167160"
---
# <a name="sb_geticon-message"></a>\_Сообщение о ПЕРЕзначке SB

Возвращает значок для части в строке состояния.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Отсчитываемый от нуля индекс части, содержащей извлекаемый значок. Если этот параметр имеет значение-1, строка состояния считается строкой состояния [простого режима](status-bars.md) .

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает маркер для значка в случае успеха или **значение NULL** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





