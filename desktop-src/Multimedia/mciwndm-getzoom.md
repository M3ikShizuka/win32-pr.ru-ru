---
title: Сообщение MCIWNDM_GETZOOM (VFW. h)
description: Сообщение МЦИВНДМ \_ Zoom получает текущее значение масштаба, используемое устройством MCI. Это сообщение можно отправить явно или с помощью макроса МЦивнджетзум.
ms.assetid: 92db8df2-515a-4616-a0f5-245d466ba379
keywords:
- сообщение MCIWNDM_GETZOOM Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_GETZOOM
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: fcb4ae1883787f1b86dcc17f2d4a3e0e0ee29ced
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370689"
---
# <a name="mciwndm_getzoom-message"></a>\_Сообщение МЦИВНДМ Zoom

Сообщение **МЦИВНДМ \_ Zoom** получает текущее значение масштаба, используемое устройством MCI. Это сообщение можно отправить явно или с помощью макроса [**мЦивнджетзум**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetzoom) .


```C++
MCIWNDM_GETZOOM 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает последние значения, используемые с [**мЦивндм \_ сетзум**](mciwndm-setzoom.md).

## <a name="remarks"></a>Remarks

Возвращаемое значение 100 означает, что изображение не масштабируется. Значение 200 указывает, что изображение увеличивается вдвое в два раза. Значение 50 указывает, что изображение уменьшается до половины исходного размера.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**мЦивнджетзум**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetzoom)
</dt> <dt>

[**МЦИВНДМ \_ сетзум**](mciwndm-setzoom.md)
</dt> </dl>

 

 





