---
title: Сообщение LVM_GETBKIMAGE (Коммктрл. h)
description: Возвращает фоновое изображение в элементе управления "представление списка". Это сообщение можно отправить явно или с помощью \_ макроса Жетбкимаже ListView.
ms.assetid: db0e8f31-746a-4a16-b689-68da696e3657
keywords:
- элементы управления Windows сообщений LVM_GETBKIMAGE
topic_type:
- apiref
api_name:
- LVM_GETBKIMAGE
- LVM_GETBKIMAGEA
- LVM_GETBKIMAGEW
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c3393c226c250de2821d7fab930f950ff5a223218a77a1b9c4bc20b51b527a58
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120062644"
---
# <a name="lvm_getbkimage-message"></a>\_Сообщение LVM жетбкимаже

Возвращает фоновое изображение в элементе управления "представление списка". Это сообщение можно отправить явно или с помощью макроса [**\_ жетбкимаже ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_getbkimage) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**лвбкимаже**](/windows/win32/api/commctrl/ns-commctrl-lvbkimagea) , которая получит сведения о фоновом изображении.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ненулевое значение в случае успеха или ноль в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **LVM \_ ЖЕТБКИМАЖЕВ** (Юникод) и **LVM \_ жетбкимажеа** (ANSI)<br/>             |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**LVM \_ сетбкимаже**](lvm-setbkimage.md)
</dt> </dl>

 

 





