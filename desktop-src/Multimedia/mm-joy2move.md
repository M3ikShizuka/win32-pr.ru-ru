---
title: Сообщение MM_JOY2MOVE (Ммсистем. h)
description: '\_Сообщение JOY2MOVE mm уведомляет окно с захваченным джойстиком, JOYSTICKID2, что расположение джойстика изменилось.'
ms.assetid: 8dc1c092-3947-43d5-8504-a4e4e121fbcb
keywords:
- сообщение MM_JOY2MOVE Windows мультимедиа
topic_type:
- apiref
api_name:
- MM_JOY2MOVE
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ec8921f0ae76d05c429d6750944a26662c1276af
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127265960"
---
# <a name="mm_joy2move-message"></a>MM \_ JOY2MOVE, сообщение

Сообщение **\_ JOY2MOVE mm** уведомляет окно с захваченным джойстиком, JOYSTICKID2, что расположение джойстика изменилось.


```C++
MM_JOY2MOVE 
fwButtons = wParam; 
xPos = LOWORD(lParam); 
yPos = HIWORD(lParam); 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="fwButtons"></span><span id="fwbuttons"></span><span id="FWBUTTONS"></span>*фвбуттонс*
</dt> <dd>

Определяет нажатые кнопки. Это может быть одно или несколько из следующих значений:



| Требование | Значение |
|--------------|------------------------------------|
| РАДОСТЬ \_ | Нажата первая кнопка джойстика.  |
| ДЖОЙСТИК ( \_ Button2) | Нажата вторая кнопка джойстика. |
| \_BUTTON3 радости | Нажата третья кнопка джойстика.  |
| \_BUTTON4 радости | Нажата четвертая кнопка джойстика. |



 

</dd> <dt>

<span id="xPos"></span><span id="xpos"></span><span id="XPOS"></span>*кспос*
</dt> <dd>

Координаты x джойстика относительно левого верхнего угла клиентской области.

</dd> <dt>

<span id="yPos"></span><span id="ypos"></span><span id="YPOS"></span>*ипос*
</dt> <dd>

Координата по оси y джойстика относительно левого верхнего угла клиентской области.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>ммсистем. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Джойстики](joysticks.md)
</dt> <dt>

[Мультимедийные сообщения джойстика](multimedia-joystick-messages.md)
</dt> </dl>

 

 





