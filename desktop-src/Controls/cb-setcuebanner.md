---
title: Сообщение CB_SETCUEBANNER (Winuser. h)
description: Задает текст баннера подсказки, отображаемый для элемента управления "поле ввода" поля со списком.
ms.assetid: 4b2b5042-ba64-4e3f-adeb-9aea66773b0e
keywords:
- элементы управления Windows сообщений CB_SETCUEBANNER
topic_type:
- apiref
api_name:
- CB_SETCUEBANNER
api_location:
- CommCtrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d5799b1b1be5e938ce1e234948a1f7d878122f30
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127174176"
---
# <a name="cb_setcuebanner-message"></a>\_Сообщение СЕТКУЕБАННЕР CB

Задает текст баннера подсказки, отображаемый для элемента управления "поле ввода" поля со списком.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на завершающийся нулем буфер строки в Юникоде, содержащий текст.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает 1 в случае успеха или значение ошибки в противном случае.

## <a name="remarks"></a>Remarks

Баннер подсказки — это текст, отображаемый в элементе управления "поле со списком" при отсутствии выделения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Возможности поля со списком](combo-box-features.md)
</dt> </dl>

 

 





