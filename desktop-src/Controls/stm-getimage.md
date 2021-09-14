---
title: Сообщение STM_GETIMAGE (Winuser. h)
description: Приложение отправляет сообщение STM- \_ Image для получения маркера изображения (значка или точечного рисунка), связанного со статическим элементом управления.
ms.assetid: eb5fe67a-09be-4c13-89c6-0e2f23e8c081
keywords:
- элементы управления Windows сообщений STM_GETIMAGE
topic_type:
- apiref
api_name:
- STM_GETIMAGE
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 77fe0c3d00a2a957530160a5ce5a21b8a1cf84e9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167003"
---
# <a name="stm_getimage-message"></a>\_Сообщение STM

Приложение отправляет сообщение **STM- \_ Image** для получения маркера изображения (значка или точечного рисунка), связанного со статическим элементом управления.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Указывает тип извлекаемого изображения. Этот параметр может принимать одно из следующих значений:



| Значение                                                                                                                                                                     | Значение                       |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------|
| <span id="IMAGE_BITMAP"></span><span id="image_bitmap"></span><dl> <dt>**\_точечный рисунок изображения**</dt> </dl>                | Массив.<br/>            |
| <span id="IMAGE_CURSOR"></span><span id="image_cursor"></span><dl> <dt>**\_курсор изображения**</dt> </dl>                | Набора.<br/>            |
| <span id="IMAGE_ENHMETAFILE"></span><span id="image_enhmetafile"></span><dl> <dt>**\_ЕНХМЕТАФИЛЕ изображения**</dt> </dl> | Расширенный метафайл.<br/> |
| <span id="IMAGE_ICON"></span><span id="image_icon"></span><dl> <dt>**\_значок изображения**</dt> </dl>                      | Значок.<br/>              |



 

</dd> <dt>

*lParam* 
</dt> <dd>

Этот параметр не используется.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение — это обработчик изображения, если таковой имеется; в противном случае он имеет **значение NULL**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**STM \_ сетимаже**](stm-setimage.md)
</dt> </dl>

 

 





