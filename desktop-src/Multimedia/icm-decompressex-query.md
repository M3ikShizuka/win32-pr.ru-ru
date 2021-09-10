---
title: Сообщение ICM_DECOMPRESSEX_QUERY (VFW. h)
description: Сообщение с \_ \_ запросом ICM декомпрессекс запрашивает драйвер сжатия видео, чтобы определить, поддерживает ли он определенный входной формат, или же он может распаковать определенный входной формат в определенный выходной формат.
ms.assetid: 7778a52d-2ed8-495c-8656-c6beb1863499
keywords:
- сообщение ICM_DECOMPRESSEX_QUERY Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_DECOMPRESSEX_QUERY
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4e5b2ef5999b9e0619ccbd9ccabd9bc5223b3bf2
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370524"
---
# <a name="icm_decompressex_query-message"></a>\_ \_ Сообщение запроса ICM декомпрессекс

Сообщение **с \_ \_ запросом ICM декомпрессекс** запрашивает драйвер сжатия видео, чтобы определить, поддерживает ли он определенный входной формат, или же он может распаковать определенный входной формат в определенный выходной формат.


```C++
ICM_DECOMPRESSEX_QUERY 
wParam = (DWORD_PTR) (LPVOID) &icdex; 
lParam = sizeof(ICDECOMPRESSEX); 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="icdex"></span><span id="ICDEX"></span>*икдекс*
</dt> <dd>

Указатель на структуру [**икдекомпрессекс**](/windows/desktop/api/Vfw/ns-vfw-icdecompressex) , содержащую входной формат.

</dd> <dt>

<span id="lParam"></span><span id="lparam"></span><span id="LPARAM"></span>*lParam*
</dt> <dd>

Размер [**икдекомпрессекс**](/windows/desktop/api/Vfw/ns-vfw-icdecompressex)в байтах.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ИЦЕРР \_ ОК, если указанное распаковка поддерживается или ицерр \_ бадформат в противном случае.

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

 

 





