---
title: Сообщение TVM_ENDEDITLABELNOW (Коммктрл. h)
description: Завершает редактирование метки элемента древовидного представления. Это сообщение можно отправить явно или с помощью \_ макроса Ендедитлабелнов TreeView.
ms.assetid: 68de2020-9311-4958-859a-de55f5e41fcf
keywords:
- элементы управления Windows сообщений TVM_ENDEDITLABELNOW
topic_type:
- apiref
api_name:
- TVM_ENDEDITLABELNOW
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4f059be20560adeb8cbcb0c63a2555283f6b7051
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165784"
---
# <a name="tvm_endeditlabelnow-message"></a>\_Сообщение TVM ендедитлабелнов

Завершает редактирование метки элемента древовидного представления. Это сообщение можно отправить явно или с помощью макроса [**\_ ендедитлабелнов TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_endeditlabelnow) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Переменная, которая указывает, отменяется ли редактирование без сохранения в метке. Если этот параметр имеет **значение true**, система отменяет редактирование без сохранения изменений. В противном случае система сохранит изменения в метке.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="remarks"></a>Remarks

Это сообщение вызывает отправку кода уведомления [ТВН \_ ендлабеледит](tvn-endlabeledit.md) в родительское окно элемента управления "дерево-представление".

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





