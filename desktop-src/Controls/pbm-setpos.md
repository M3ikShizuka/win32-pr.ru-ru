---
title: Сообщение PBM_SETPOS (Коммктрл. h)
description: Задает текущую точку для индикатора выполнения и перерисовывает линию для отражения новой должности.
ms.assetid: 9ebeaa19-0f42-4af7-85d8-aae22498fd6f
keywords:
- элементы управления Windows сообщений PBM_SETPOS
topic_type:
- apiref
api_name:
- PBM_SETPOS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1bf9c6a4c21439f93f3459a5061daf28192081a042cc663a644110a1e54d2c54
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119986154"
---
# <a name="pbm_setpos-message"></a>\_Сообщение СЕТПОС PBM

Задает текущую точку для индикатора выполнения и перерисовывает линию для отражения новой должности.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Целое число со знаком, которое станет новой позицией.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает предыдущее расположение.

## <a name="remarks"></a>Remarks

Если параметр *wParam* находится за пределами диапазона элемента управления, то в качестве расположения устанавливается Ближайшая граница.

Не отправляйте это сообщение элементу управления с стилем [**\_ области PBS**](progress-bar-control-styles.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





