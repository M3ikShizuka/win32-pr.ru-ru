---
title: Сообщение EM_GETOPTIONS (RichEdit. h)
description: Возвращает широкие параметры элемента управления редактированием.
ms.assetid: 183f0fed-8666-4ed5-ac48-362c818378d2
keywords:
- элементы управления Windows сообщений EM_GETOPTIONS
topic_type:
- apiref
api_name:
- EM_GETOPTIONS
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6b31af3663331b63553fc262fc9bdbd5613c5768
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170059"
---
# <a name="em_getoptions-message"></a>\_Сообщение о параметре EM

Возвращает широкие параметры элемента управления редактированием.

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

Это сообщение Возвращает сочетание текущих значений флагов параметров, описанных в сообщении [**EM \_ сетоптионс**](em-setoptions.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**EM \_ сетоптионс**](em-setoptions.md)
</dt> </dl>

 

 





