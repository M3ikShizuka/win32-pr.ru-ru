---
title: Сообщение RB_GETBARINFO (Коммктрл. h)
description: Извлекает сведения об элементе управления "Главная панель" и используемом в нем списке изображений.
ms.assetid: d3d56b95-7540-4e45-bb2e-b9d41cfcca0d
keywords:
- элементы управления Windows сообщений RB_GETBARINFO
topic_type:
- apiref
api_name:
- RB_GETBARINFO
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 58d1d1ee657f88b95b0caad254377ebca0db74b313fd7eb3fe102d4f488c14d1
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120085094"
---
# <a name="rb_getbarinfo-message"></a>\_Сообщение ЖЕТБАРИНФО RB

Извлекает сведения об элементе управления "Главная панель" и используемом в нем списке изображений.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**ребаринфо**](/windows/win32/api/commctrl/ns-commctrl-rebarinfo) , которая будет принимать сведения об элементе управления главной панели. Перед отправкой этого сообщения необходимо задать для элемента **кбсизе** этой структуры значение **sizeof**(ребаринфо).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ненулевое значение в случае успеха или ноль в противном случае.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





