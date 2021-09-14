---
title: Сообщение BM_SETSTYLE (Winuser. h)
description: Задает стиль кнопки. Это сообщение можно отправить явным образом или воспользоваться \_ макросом кнопки SetStyle.
ms.assetid: 6439e68f-87fc-4a4a-8025-facc3c0e03e2
keywords:
- элементы управления Windows сообщений BM_SETSTYLE
topic_type:
- apiref
api_name:
- BM_SETSTYLE
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3c080e1098d70b17e1e68bbbcd2d5598db79ef8f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054488"
---
# <a name="bm_setstyle-message"></a>\_Сообщение BM SETSTYLE

Задает стиль кнопки. Это сообщение можно отправить явным образом или воспользоваться макросом [**кнопки \_ SetStyle**](/windows/desktop/api/Windowsx/nf-windowsx-button_setstyle) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Стиль кнопки. Этот параметр может быть сочетанием стилей кнопок. Таблицу стилей кнопок см. в разделе [стили кнопок](button-styles.md).

</dd> <dt>

*lParam* 
</dt> <dd>

[**Ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85)) объекта *lParam* — это **логическое** значение, указывающее, следует ли перерисовать кнопку. Значение **true** Перерисовывает кнопку; значение **false** не перерисовывает кнопку.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение всегда возвращает ноль.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



 

