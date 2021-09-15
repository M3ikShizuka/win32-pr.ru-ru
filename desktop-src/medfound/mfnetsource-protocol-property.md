---
description: Указывает протокол управления, используемый сетевым источником.
ms.assetid: 4de8b8ba-97d9-4269-a16c-1853dc02f674
title: Свойство MFNETSOURCE_PROTOCOL (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b188eeb1f6669544291f4dca95db8a4a45a50d7b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574874"
---
# <a name="mfnetsource_protocol-property"></a>\_Свойство протокола мфнетсаурце

Указывает протокол управления, используемый сетевым источником. Значение этого свойства является членом перечисления [**\_ \_ типа протокола мфнетсаурце**](/windows/desktop/api/mfidl/ne-mfidl-mfnetsource_protocol_type) .



Тип данных

Тип ПРОПВАРИАНТ (VT)

ПРОПВАРИАНТ, элемент

**LONG**

VT \_ I4

**лвал**



## <a name="remarks"></a>Комментарии

Постоянный **\_ протокол мфнетсаурце** определяет идентификатор GUID для этого ключа свойства. Идентификатор свойства (PID) равен нулю.

Это свойство доступно только для чтения. Чтобы получить это свойство, выполните запрос к источнику сети для интерфейса **ипропертисторе** и вызовите метод **Ипропертисторе:: GetValue**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> <dt>

[Сетевые подключения в Media Foundation](networking-in-media-foundation.md)
</dt> <dt>

[Поддерживаемые протоколы](supported-protocols.md)
</dt> </dl>

 

 




