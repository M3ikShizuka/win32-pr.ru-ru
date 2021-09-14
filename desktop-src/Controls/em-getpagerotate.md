---
title: Сообщение EM_GETPAGEROTATE (RichEdit. h)
description: Возвращает макет текста для элемента управления Microsoft Rich Edit.
ms.assetid: 0efb112e-ad51-4ebb-9037-3aee3ab9ad1d
keywords:
- элементы управления Windows сообщений EM_GETPAGEROTATE
topic_type:
- apiref
api_name:
- EM_GETPAGEROTATE
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ad7bc7cd3c77ae88cd4c8710e14b4472e57407ca
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170052"
---
# <a name="em_getpagerotate-message"></a>\_Сообщение ЖЕТПАЖЕРОТАТЕ EM

\[**EM \_ ЖЕТПАЖЕРОТАТЕ** доступен для использования в операционных системах, указанных в разделе требования. В последующих версиях он может быть изменен или недоступен.\]

Возвращает макет текста для элемента управления Microsoft Rich Edit.

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

Возвращает текущий макет текста. Список возможных значений макета текста см. в разделе [**EM \_ сетпажеротате**](em-setpagerotate.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP с пакетом обновления 1 (SP1), \[ только классические приложения\]<br/>                                  |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**EM \_ сетпажеротате**](em-setpagerotate.md)
</dt> </dl>

 

 





