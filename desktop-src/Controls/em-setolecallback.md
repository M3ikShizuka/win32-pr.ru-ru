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
ms.openlocfilehash: 9a7b16494bf0e34606809d5b4670a05d4ae3c60a6ea49c8103688c6e09676c98
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120048304"
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

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



 

