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
ms.openlocfilehash: d8a157f6a220f4932d39d13f08df79afa99d7348
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167748"
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



 

 





