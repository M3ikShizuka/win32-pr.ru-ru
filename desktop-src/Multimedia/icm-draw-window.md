---
title: Сообщение ICM_DRAW_WINDOW (VFW. h)
description: Сообщение в \_ окне ICM Draw \_ уведомляет драйвер подготовки, что необходимо перерисовать окно, заданное для \_ \_ начала сообщения ICM Draw.
ms.assetid: 4df1b9a7-8d61-4e79-8f43-1e7ee266375c
keywords:
- сообщение ICM_DRAW_WINDOW Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_DRAW_WINDOW
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1a1f66ca5beefa3d7eb774174bccc9d9482aebddd4a82341e9c83bb265d7788e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119690926"
---
# <a name="icm_draw_window-message"></a>\_ \_ Сообщение окна ICM Draw

Сообщение **в \_ \_ окне ICM Draw** уведомляет драйвер подготовки, что необходимо перерисовать окно, заданное для [**\_ \_ начала сообщения ICM Draw**](icm-draw-begin.md) . Окно перемещено или временно скрыто. Это сообщение можно отправить явно или с помощью макроса [**икдраввиндов**](/windows/desktop/api/Vfw/nf-vfw-icdrawwindow) .


```C++
ICM_DRAW_WINDOW 
wParam = (DWORD_PTR) (LPVOID) prc; 
lParam = 0; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="prc"></span><span id="PRC"></span>*PRC*
</dt> <dd>

Указатель на прямоугольник назначения в координатах экрана. Если этот параметр указывает на пустой прямоугольник, отрисовка должна быть отключена.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ИЦЕРР \_ ОК в случае успеха или ошибку в противном случае.

## <a name="remarks"></a>Remarks

Это сообщение поддерживается оборудованием, которое выполняет собственное асинхронное распаковка, время и рисование.

Драйверы наложения видео это сообщение используется для рисования при скрытии или перемещении окна. Когда окно, заданное [**для \_ \_ начала отображения ICM**](icm-draw-begin.md) , полностью скрыто другими окнами, прямоугольник назначения пуст. При возникновении этого условия драйверы должны отключать оборудование наложения видео.

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

 

 





