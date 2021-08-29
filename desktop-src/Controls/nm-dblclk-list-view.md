---
title: Код уведомления NM_DBLCLK (представление списка) (Коммктрл. h)
description: Посылается элементом управления "представление списка", когда пользователь дважды щелкает элемент с левой кнопкой мыши. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 28455109-177e-4932-88c5-500a3a91c13a
keywords:
- NM_DBLCLK (представление списка) код уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- NM_DBLCLK
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c3590b417954f67c454b6cece979bdd6eac4706fa5dfc97b7dda30be6dde183c
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119919704"
---
# <a name="nm_dblclk-list-view-notification-code"></a>\_Код уведомления NM дблклк (представление списка)

Посылается элементом управления "представление списка", когда пользователь дважды щелкает элемент с левой кнопкой мыши. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
NM_DBLCLK
        
    lpnmitem = (LPNMITEMACTIVATE) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

[Версия 4,71](common-control-versions.md). Указатель на структуру [**нмитемактивате**](/windows/win32/api/commctrl/ns-commctrl-nmitemactivate) , содержащую дополнительные сведения об этом уведомлении. Члены этой структуры **Член iItem**, **iSubItem** и **птактион** содержат сведения об элементе.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение для этого уведомления не используется.

## <a name="remarks"></a>Remarks

Элемент **Член iItem** объекта *lParam* допустим только в том случае, если была нажата метка значка или первого столбца. Чтобы определить, какой элемент выбран при нажатии на другое место в строке, отправьте сообщение [**LVM \_ субитемхиттест**](lvm-subitemhittest.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





