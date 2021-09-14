---
title: Сообщение ICM_DECOMPRESSEX_END (VFW. h)
description: '\_ \_ Сообщение об окончании ICM декомпрессекс уведомляет драйвер распаковки о завершении распаковки и освобождения ресурсов, выделенных для распаковки. Это сообщение можно отправить явно или с помощью макроса Икдекомпрессексенд.'
ms.assetid: 7ed63a4e-bb17-43a3-b593-25c4a51be942
keywords:
- сообщение ICM_DECOMPRESSEX_END Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_DECOMPRESSEX_END
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c7e96f6a069e9ed2c9c52dc2f07f1ab4c5210ecd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067686"
---
# <a name="icm_decompressex_end-message"></a>\_ \_ Сообщение об окончании ICM декомпрессекс

Сообщение **об \_ \_ окончании ICM декомпрессекс** уведомляет драйвер распаковки о завершении распаковки и освобождения ресурсов, выделенных для распаковки. Это сообщение можно отправить явно или с помощью макроса [**икдекомпрессексенд**](/windows/desktop/api/Vfw/nf-vfw-icdecompressexend) .


```C++
ICM_DECOMPRESSEX_END 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает ИЦЕРР \_ ОК в случае успеха или ошибку в противном случае.

## <a name="remarks"></a>Remarks

Драйвер освобождает все ресурсы, выделенные для сообщения [**о \_ \_ начале ICM декомпрессекс**](icm-decompressex-begin.md) .

[**ICM \_ ДЕКОМПРЕССЕКС \_ Begin**](icm-decompressex-begin.md) и **ICM \_ декомпрессекс \_ End** не вложены. Если драйвер получает **ICM \_ декомпрессекс \_ Begin** до остановки распаковки с помощью **ICM \_ декомпрессекс \_ End**, он должен перезапустить распаковку с новыми параметрами.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Диспетчер сжатия видео](video-compression-manager.md)
</dt> <dt>

[Сообщения о сжатии видео](video-compression-messages.md)
</dt> </dl>

 

 





