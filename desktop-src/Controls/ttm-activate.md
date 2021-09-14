---
title: Сообщение TTM_ACTIVATE (Коммктрл. h)
description: Активирует или деактивирует элемент управления ToolTip.
ms.assetid: f37da001-748c-4c51-bb32-dc49031ff2fb
keywords:
- элементы управления Windows сообщений TTM_ACTIVATE
topic_type:
- apiref
api_name:
- TTM_ACTIVATE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e200b769cd3d9e07cb63a5a540960bcc707f862d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165951"
---
# <a name="ttm_activate-message"></a>\_Сообщение о активации ТТМ

Активирует или деактивирует элемент управления ToolTip.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Флаг активации. Если этот параметр имеет **значение true**, элемент управления ToolTip активируется. Если значение равно **false**, элемент управления ToolTip деактивируется.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





