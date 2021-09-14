---
title: Сообщение EM_GETAUTOCORRECTPROC (RichEdit. h)
description: Возвращает указатель на определяемую приложением функцию Аутокорректпрок.
ms.assetid: 90821036-F27D-4AC3-9AB8-40A94486B938
keywords:
- элементы управления Windows сообщений EM_GETAUTOCORRECTPROC
topic_type:
- apiref
api_name:
- EM_GETAUTOCORRECTPROC
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: dc4d730d15ca8631e6d663e3d4f971f115d5c268
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054460"
---
# <a name="em_getautocorrectproc-message"></a>\_Сообщение ЖЕТАУТОКОРРЕКТПРОК EM

Возвращает указатель на определяемую приложением функцию [*аутокорректпрок*](/windows/desktop/api/Richedit/nc-richedit-autocorrectproc) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает указатель на определяемую приложением функцию [*аутокорректпрок*](/windows/desktop/api/Richedit/nc-richedit-autocorrectproc) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[*аутокорректпрок*](/windows/desktop/api/Richedit/nc-richedit-autocorrectproc)
</dt> <dt>

[**EM \_ каллаутокорректпрок**](em-callautocorrectproc.md)
</dt> <dt>

[**EM \_ сетаутокорректпрок**](em-setautocorrectproc.md)
</dt> </dl>

 

 





