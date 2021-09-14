---
title: Сообщение PBM_GETBKCOLOR (Коммктрл. h)
description: Возвращает цвет фона индикатора выполнения.
ms.assetid: 9526ed78-08d9-468f-831b-72bb7c8c92d1
keywords:
- элементы управления Windows сообщений PBM_GETBKCOLOR
topic_type:
- apiref
api_name:
- PBM_GETBKCOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2240025629bbcc242ea7ed47be2e3db42ae73b15
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167780"
---
# <a name="pbm_getbkcolor-message"></a>\_Сообщение ЖЕТБККОЛОР PBM

Возвращает цвет фона индикатора выполнения.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает цвет фона индикатора выполнения.

## <a name="remarks"></a>Remarks

Это цвет, заданный в сообщении [**\_ сетбкколор PBM**](pbm-setbkcolor.md) . Значение по умолчанию — CLR \_ по умолчанию, которое определено в коммктрл. h.

Эта функция влияет только на классический режим, а не на визуальный стиль.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





