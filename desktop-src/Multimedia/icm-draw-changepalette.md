---
title: Сообщение ICM_DRAW_CHANGEPALETTE (VFW. h)
description: Сообщение ICM \_ Draw \_ чанжепалетте уведомляет драйвер подготовки к просмотру, что изменяется палитра роликов. Это сообщение можно отправить явно или с помощью макроса Икдравчанжепалетте.
ms.assetid: 974fc0d8-d0c7-4a82-af84-68b53f753259
keywords:
- сообщение ICM_DRAW_CHANGEPALETTE Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_DRAW_CHANGEPALETTE
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6364abb2c535158b2e64ff311041b00490c5958c
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370539"
---
# <a name="icm_draw_changepalette-message"></a>\_Сообщение ICM Draw \_ чанжепалетте

Сообщение **ICM \_ Draw \_ чанжепалетте** уведомляет драйвер подготовки к просмотру, что изменяется палитра роликов. Это сообщение можно отправить явно или с помощью макроса [**икдравчанжепалетте**](/windows/desktop/api/Vfw/nf-vfw-icdrawchangepalette) .


```C++
ICM_DRAW_CHANGEPALETTE 
wParam = (DWORD_PTR) (LPVOID) lpbiInput; 
lParam = 0; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="lpbiInput"></span><span id="lpbiinput"></span><span id="LPBIINPUT"></span>*лпбиинпут*
</dt> <dd>

Указатель на структуру [**битмапинфо**](/windows/win32/api/wingdi/ns-wingdi-bitmapinfo) , содержащую новый формат и необязательную таблицу цветов.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ИЦЕРР \_ ОК в случае успеха или **false** в противном случае.

## <a name="remarks"></a>Remarks

Это сообщение должно поддерживаться с помощью устанавливаемых обработчиков отрисовки, которые рисуют DIB с внутренней структурой, содержащей палитру.

## <a name="requirements"></a>Требования



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

 

