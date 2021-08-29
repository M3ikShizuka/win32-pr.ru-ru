---
title: Сообщение TBM_GETNUMTICS (Коммктрл. h)
description: Возвращает количество делений в TrackBar.
ms.assetid: 3c3f7ebb-a544-474c-ba14-68eae543ee38
keywords:
- элементы управления Windows сообщений TBM_GETNUMTICS
topic_type:
- apiref
api_name:
- TBM_GETNUMTICS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 98d247dd49db4223cd61de3684bc2ea92d6d00c843416d4f9d5a8650e6eb8b85
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120046554"
---
# <a name="tbm_getnumtics-message"></a>\_Сообщение ТБМ жетнумтикс

Возвращает количество делений в TrackBar.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если [флаг деления](trackbar-control-styles.md) не установлен, он возвращает значение 2 для начального и конечного тактов. Если [**задан \_ параметр TBS**](trackbar-control-styles.md) , он возвращает ноль. В противном случае он принимает разность между минимальным и максимальным диапазоном, делит их на тактовую частоту и добавляет 2.

## <a name="remarks"></a>Remarks

Сообщение **ТБМ \_ жетнумтикс** подсчитывает все деления, включая первый и последний деления, созданные с помощью TrackBar.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





