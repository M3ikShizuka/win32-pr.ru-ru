---
title: Сообщение CB_GETCOMBOBOXINFO (Winuser. h)
description: Возвращает сведения об указанном поле со списком.
ms.assetid: 3239dfa8-7301-48e3-ba8e-29c5d5f43b39
keywords:
- элементы управления Windows сообщений CB_GETCOMBOBOXINFO
topic_type:
- apiref
api_name:
- CB_GETCOMBOBOXINFO
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bd7052ef4feca8a8704258c7c34d6516c7cd6cd4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173960"
---
# <a name="cb_getcomboboxinfo-message"></a>\_Сообщение ЖЕТКОМБОБОКСИНФО CB

Возвращает сведения об указанном поле со списком.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Этот параметр не используется.

</dd> <dt>

*lParam* \[ заполняет\]
</dt> <dd>

Указатель на структуру [**комбобоксинфо**](/windows/win32/api/winuser/ns-winuser-comboboxinfo) , которая получает сведения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если функция выполняется успешно, возвращается ненулевое значение.

Если функция выполняется неудачно, возвращается нулевое значение. Дополнительные сведения об ошибке можно получить, вызвав [**GetLastError**](/windows/desktop/api/errhandlingapi/nf-errhandlingapi-getlasterror).

## <a name="remarks"></a>Комментарии

Это сообщение эквивалентно [**жеткомбобоксинфо**](/windows/desktop/api/Winuser/nf-winuser-getcomboboxinfo).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[**комбобоксинфо**](/windows/win32/api/winuser/ns-winuser-comboboxinfo)
</dt> <dt>

[**жеткомбобоксинфо**](/windows/desktop/api/Winuser/nf-winuser-getcomboboxinfo)
</dt> </dl>

 

