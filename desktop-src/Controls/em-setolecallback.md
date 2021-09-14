---
title: Сообщение EM_SETOLECALLBACK (RichEdit. h)
description: Предоставляет форматируемый элемент управления "поле ввода", объект Иричедитолекаллбакк, используемый элементом управления для получения связанных с OLE ресурсов и информации от клиента.
ms.assetid: bd1f8048-214c-4ac6-b826-bedabb1aaee5
keywords:
- элементы управления Windows сообщений EM_SETOLECALLBACK
topic_type:
- apiref
api_name:
- EM_SETOLECALLBACK
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: edfc54db112bba42fc3d51b2e328fc7641990c7f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054339"
---
# <a name="em_setolecallback-message"></a>\_Сообщение СЕТОЛЕКАЛЛБАКК EM

Предоставляет форматируемый элемент управления "поле ввода", объект [**иричедитолекаллбакк**](/windows/desktop/api/Richole/nn-richole-iricheditolecallback) , используемый элементом управления для получения связанных с OLE ресурсов и информации от клиента.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Этот параметр не используется; оно должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на объект [**иричедитолекаллбакк**](/windows/desktop/api/Richole/nn-richole-iricheditolecallback) . Перед возвратом элемент управления вызывает метод [**AddRef**](/windows/desktop/api/unknwn/nf-unknwn-iunknown-addref) для объекта.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если операция завершилась удачно, возвращаемое значение будет ненулевым.

Если операция завершается ошибкой, возвращаемое значение равно нулю.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



 

