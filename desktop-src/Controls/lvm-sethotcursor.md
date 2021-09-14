---
title: Сообщение LVM_SETHOTCURSOR (Коммктрл. h)
description: Задает значение ХКУРСОР, которое используется элементом управления "представление списка" при наведении указателя мыши на элемент, пока включено отслеживание.
ms.assetid: e3ff8608-9389-4167-839b-ecc2be01bb64
keywords:
- элементы управления Windows сообщений LVM_SETHOTCURSOR
topic_type:
- apiref
api_name:
- LVM_SETHOTCURSOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0e743f74eda3b59f04f6f4793b47d76da3bab881
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126972061"
---
# <a name="lvm_sethotcursor-message"></a>\_Сообщение LVM сесоткурсор

Задает значение ХКУРСОР, которое используется элементом управления "представление списка" при наведении указателя мыши на элемент, пока включено отслеживание. Это сообщение можно отправить явным образом или использовать макрос [**\_ сесоткурсор ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_sethotcursor) . Чтобы проверить, включено ли оперативное отслеживание, вызовите [**системпараметерсинфо**](/windows/desktop/api/winuser/nf-winuser-systemparametersinfoa).

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на заданный курсор.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение ХКУРСОР, которое является предыдущим активным курсором.

## <a name="remarks"></a>Комментарии

Элемент управления "представление списка" использует функцию отслеживания и выбора при наведении указателя, если установлен стиль [**LVS \_ ex \_ траккселект**](extended-list-view-styles.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

