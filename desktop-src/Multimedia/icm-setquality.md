---
title: Сообщение ICM_SETQUALITY (VFW. h)
description: Сообщение ICM \_ сеткуалити предоставляет драйверу сжатия видео с уровнем качества, который будет использоваться во время сжатия.
ms.assetid: 487ff1de-7178-440a-b38d-0b82a30d7297
keywords:
- сообщение ICM_SETQUALITY Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_SETQUALITY
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: adb840b3dc283d0cd81b4662322e0571b8e687bbdd4b6e7009a6fa1786e95920
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119784914"
---
# <a name="icm_setquality-message"></a>\_Сообщение ICM сеткуалити

Сообщение **ICM \_ сеткуалити** предоставляет драйверу сжатия видео с уровнем качества, который будет использоваться во время сжатия.


```C++
ICM_SETQUALITY 
wParam = (DWORD) (LPVOID) &dwICValue; 
lParam = 0; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="dwICValue"></span><span id="dwicvalue"></span><span id="DWICVALUE"></span>*двиквалуе*
</dt> <dd>

Новое значение качества. Значения качества находятся в диапазоне от 0 до 10 000.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ИЦЕРР \_ ОК, если драйвер поддерживает это сообщение или ИЦЕРР \_ не поддерживается в противном случае.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Диспетчер сжатия видео](video-compression-manager.md)
</dt> <dt>

[Сообщения о сжатии видео](video-compression-messages.md)
</dt> </dl>

 

 





