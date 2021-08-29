---
title: Сообщение TVM_GETITEMHEIGHT (Коммктрл. h)
description: Извлекает текущую высоту каждого элемента представления дерева. Это сообщение можно отправить явно или с помощью \_ макроса GetItemHeight TreeView.
ms.assetid: 017476a3-1929-4a31-97a7-0f66175d47ea
keywords:
- элементы управления Windows сообщений TVM_GETITEMHEIGHT
topic_type:
- apiref
api_name:
- TVM_GETITEMHEIGHT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 960e5f8c8651d9a18b40741e7888d325df5f011efacdcc0f629b52c7aab4a6bd
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120045794"
---
# <a name="tvm_getitemheight-message"></a>\_Сообщение TVM GETITEMHEIGHT

Извлекает текущую высоту каждого элемента представления дерева. Это сообщение можно отправить явно или с помощью макроса [**\_ GetItemHeight TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_getitemheight) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает высоту каждого элемента в пикселях.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**TVM \_ сетитемхеигхт**](tvm-setitemheight.md)
</dt> </dl>

 

 





