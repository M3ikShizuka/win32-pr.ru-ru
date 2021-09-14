---
title: Сообщение ICM_GETINFO (VFW. h)
description: Сообщение ICM \_ info запрашивает драйвер сжатия видео, чтобы получить описание самого себя в структуре иЦинфо.
ms.assetid: 8029f247-9777-4a34-9e84-908482094493
keywords:
- сообщение ICM_GETINFO Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_GETINFO
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 634803b7dd9a3b8900c35fabedcadb99908c2b31
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246262"
---
# <a name="icm_getinfo-message"></a>Информационное \_ сообщение ICM

Сообщение **ICM \_ info** запрашивает драйвер сжатия видео, чтобы получить описание самого себя в структуре [**иЦинфо**](/windows/desktop/api/Vfw/ns-vfw-icinfo) .


```C++
ICM_GETINFO 
wParam = (DWORD) (LPVOID) lpicinfo; 
lParam = sizeof(ICINFO); 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="lpicinfo"></span><span id="LPICINFO"></span>*лпиЦинфо*
</dt> <dd>

Указатель на структуру **иЦинфо** для хранения информации.

</dd> <dt>

<span id="lParam"></span><span id="lparam"></span><span id="LPARAM"></span>*lParam*
</dt> <dd>

Размер **иЦинфо** в байтах.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает размер (в байтах) [**иЦинфо**](/windows/desktop/api/Vfw/ns-vfw-icinfo) или нуль в случае возникновения ошибки.

## <a name="remarks"></a>Remarks

Как правило, приложения отправляют это сообщение, чтобы отобразить список установленных компрессоров.

Драйвер должен заполнить все элементы структуры [**иЦинфо**](/windows/desktop/api/Vfw/ns-vfw-icinfo) , за исключением **сздривер**.

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

 

 





