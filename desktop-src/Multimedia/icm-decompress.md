---
title: Сообщение ICM_DECOMPRESS (VFW. h)
description: Сообщение ICM \_ uncompression уведомляет драйвер распаковки видео о необходимости распаковки кадра данных в буфер, определенный приложением.
ms.assetid: 666f2ebf-80a5-4846-861d-c79c3001c5a0
keywords:
- сообщение ICM_DECOMPRESS Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_DECOMPRESS
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0c890a8ca15202f57fdaa02922e364af75f7b952
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067688"
---
# <a name="icm_decompress-message"></a>\_Сообщение распаковки ICM

Сообщение **ICM \_** uncompression уведомляет драйвер распаковки видео о необходимости распаковки кадра данных в буфер, определенный приложением.


```C++
ICM_DECOMPRESS 
wParam = (DWORD) (LPVOID) &icd; 
lParam = sizeof(ICDECOMPRESS); 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="icd"></span><span id="ICD"></span>*ICD*
</dt> <dd>

Указатель на структуру [**икдекомпресс**](/windows/desktop/api/Vfw/ns-vfw-icdecompress) .

</dd> <dt>

<span id="lParam"></span><span id="lparam"></span><span id="LPARAM"></span>*lParam*
</dt> <dd>

Размер [**икдекомпресс**](/windows/desktop/api/Vfw/ns-vfw-icdecompress)в байтах.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ИЦЕРР \_ ОК в случае успеха или ошибку в противном случае.

## <a name="remarks"></a>Remarks

Если требуется, чтобы драйвер распаковать данные непосредственно на экране, отправьте сообщение [**ICM \_ Draw**](icm-draw.md) .

Драйвер возвращает ошибку, если это сообщение получено до сообщения [**\_ \_ начала распаковки ICM**](icm-decompress-begin.md) .

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

 

 





