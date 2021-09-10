---
title: Сообщение ICM_DRAW_END (VFW. h)
description: '\_ \_ Сообщение о ЗАВЕРШЕНии ICM выводит драйвер подготовки к распаковке текущего изображения на экран и освобождения ресурсов, выделенных для распаковки и рисования. Это сообщение можно отправить явно или с помощью макроса Икдравенд.'
ms.assetid: 03910752-6122-4a5a-84ff-2cecf66cf439
keywords:
- сообщение ICM_DRAW_END Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_DRAW_END
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e420ac37791bc6c5aa7f660d71005be65fc87fff
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370521"
---
# <a name="icm_draw_end-message"></a>\_Сообщение окончания прорисовки ICM \_

Сообщение **о \_ \_ завершении ICM** выводит драйвер подготовки к распаковке текущего изображения на экран и освобождения ресурсов, выделенных для распаковки и рисования. Это сообщение можно отправить явно или с помощью макроса [**икдравенд**](/windows/desktop/api/Vfw/nf-vfw-icdrawend) .


```C++
ICM_DRAW_END 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает ИЦЕРР \_ ОК в случае успеха или ошибку в противном случае.

## <a name="remarks"></a>Remarks

[**\_ \_ Начало**](icm-draw-begin.md) и **\_ \_ конец** изображения ICM не вложены в сообщения. Если драйвер получает функцию **ICM \_ Draw \_** , то перед **\_ \_ завершением** распаковки с использованием ICM Draw необходимо перезапустить распаковку с новыми параметрами.

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

 

 





