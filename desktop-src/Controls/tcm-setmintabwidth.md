---
title: Сообщение TCM_SETMINTABWIDTH (Коммктрл. h)
description: Устанавливает минимальную ширину элементов в элементе управления "Вкладка". Это сообщение можно отправить явным образом или с помощью \_ макроса табктрл сетминтабвидс.
ms.assetid: c0be3d4e-774c-4233-820f-01ffbb69ecf0
keywords:
- элементы управления Windows сообщений TCM_SETMINTABWIDTH
topic_type:
- apiref
api_name:
- TCM_SETMINTABWIDTH
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1136afa6952c30c51b619636e938b7887cd9dcf55da8d3f2d9c585ba9e1d82c1
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120104704"
---
# <a name="tcm_setmintabwidth-message"></a>\_Сообщение СЕТМИНТАБВИДС TCM

Устанавливает минимальную ширину элементов в элементе управления "Вкладка". Это сообщение можно отправить явным образом или с помощью макроса [**табктрл \_ сетминтабвидс**](/windows/desktop/api/Commctrl/nf-commctrl-tabctrl_setmintabwidth) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Минимальная ширина, устанавливаемая для элемента управления вкладки. Если этот параметр имеет значение-1, то элемент управления будет использовать ширину табуляции по умолчанию.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение типа INT, представляющее предыдущую минимальную ширину табуляции.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





