---
title: Сообщение TVM_GETTOOLTIPS (Коммктрл. h)
description: Получает маркер для дочернего элемента управления ToolTip, используемого элементом управления "дерево-представление". Это сообщение можно отправить явным образом или с помощью \_ макроса TreeView.
ms.assetid: 65e8189e-ae3e-4268-b1ed-bb0d88f2cbe3
keywords:
- элементы управления Windows сообщений TVM_GETTOOLTIPS
topic_type:
- apiref
api_name:
- TVM_GETTOOLTIPS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9f0166402c7605139d3e27fce17b94ad0afdffb66622f40da4adc3044b7023d8
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120060174"
---
# <a name="tvm_gettooltips-message"></a>Сообщение TVM с \_ ПОДсказками

Получает маркер для дочернего элемента управления ToolTip, используемого элементом управления "дерево-представление". Это сообщение можно отправить явным образом или с помощью макроса [**TreeView \_**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_gettooltips) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает указатель на дочерний элемент управления ToolTip или **значение NULL** , если элемент управления не использует подсказки.

## <a name="remarks"></a>Remarks

При создании элементы управления "представление в виде дерева" автоматически создают дочерний элемент управления ToolTip. Чтобы элемент управления "дерево" не использовал подсказки, создайте элемент управления с стилем " [**\_ подсказки" телевизоров**](tree-view-control-window-styles.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**TVM \_ сеттултипс**](tvm-settooltips.md)
</dt> </dl>

 

 





