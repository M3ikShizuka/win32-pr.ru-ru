---
description: Указывает, включен ли транспорт UDP в сетевом источнике.
ms.assetid: d46a59e6-8abc-484b-aecc-edf57ffff512
title: Свойство MFNETSOURCE_ENABLE_UDP (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d326cbd375a7d7e22ea2afc121dd4af9086e60c5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127269040"
---
# <a name="mfnetsource_enable_udp-property"></a>МФНЕТСАУРЦЕ \_ включить \_ свойство UDP

Указывает, включен ли транспорт UDP в сетевом источнике.



Тип данных

Тип ПРОПВАРИАНТ (VT)

ПРОПВАРИАНТ, элемент

Логическое значение (**Long**)

VT \_ I4

**лвал**



## <a name="remarks"></a>Remarks

Константа **мфнетсаурце \_ Enable \_ UDP** определяет идентификатор GUID для этого ключа свойства. Идентификатор свойства (PID) равен нулю.

Приложения могут использовать это свойство для настройки сетевого источника. Чтобы задать свойство, передайте указатель **ипропертисторе** в сопоставитель источника. Дополнительные сведения см. [в разделе Настройка источника мультимедиа](configuring-a-media-source.md).

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

 

 




