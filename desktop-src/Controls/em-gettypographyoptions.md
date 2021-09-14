---
title: Сообщение EM_GETTYPOGRAPHYOPTIONS (RichEdit. h)
description: Возвращает текущее состояние типографских параметров элемента управления Rich Edit.
ms.assetid: 6ff5980e-3201-4b0f-9a03-3de78730ce33
keywords:
- элементы управления Windows сообщений EM_GETTYPOGRAPHYOPTIONS
topic_type:
- apiref
api_name:
- EM_GETTYPOGRAPHYOPTIONS
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6d692639ba6c8cea758abe694faed3a46e3f65be
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054428"
---
# <a name="em_gettypographyoptions-message"></a>\_Сообщение ЖЕТТИПОГРАФЙОПТИОНС EM

Возвращает текущее состояние типографских параметров элемента управления Rich Edit.

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

Возвращает текущие параметры оформления. Список параметров см. в разделе [**EM \_ сеттипографйоптионс**](em-settypographyoptions.md).

## <a name="remarks"></a>Комментарии

Вы можете включить дополнительные разрывы строк, отправив сообщение [**EM \_ сеттипографйоптионс**](em-settypographyoptions.md) . Расширенные и нормальные разрывы строк также можно включить автоматически с помощью элемента управления Rich Edit, если это необходимо для определенных языков.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Распространяемые компоненты<br/>          | Расширенное редактирование 3,0<br/>                                                              |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[**EM \_ сеттипографйоптионс**](em-settypographyoptions.md)
</dt> <dt>

**Основные понятия**
</dt> <dt>

[Общие сведения об элементах управления "поле ввода"](about-rich-edit-controls.md)
</dt> </dl>

 

 





