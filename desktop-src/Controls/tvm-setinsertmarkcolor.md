---
title: Сообщение TVM_SETINSERTMARKCOLOR (Коммктрл. h)
description: Задает цвет, используемый для отображения метки вставки для представления в виде дерева. Это сообщение можно отправить явно или с помощью \_ макроса Сетинсертмаркколор TreeView.
ms.assetid: c82304a8-3726-42c0-81e7-90d8f8205ead
keywords:
- элементы управления Windows сообщений TVM_SETINSERTMARKCOLOR
topic_type:
- apiref
api_name:
- TVM_SETINSERTMARKCOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 92668b1137b089f9a09cc9a34d63d472742bce4d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165640"
---
# <a name="tvm_setinsertmarkcolor-message"></a>\_Сообщение TVM сетинсертмаркколор

Задает цвет, используемый для отображения метки вставки для представления в виде дерева. Это сообщение можно отправить явно или с помощью макроса [**\_ сетинсертмаркколор TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_setinsertmarkcolor) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Значение [**COLORREF**](/windows/desktop/gdi/colorref) , содержащее новый цвет метки вставки.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **COLORREF** , содержащее предыдущий цвет отметки вставки.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**TVM \_ жетинсертмаркколор**](tvm-getinsertmarkcolor.md)
</dt> </dl>

 

