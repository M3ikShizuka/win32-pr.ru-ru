---
title: Сообщение ICM_GET (VFW. h)
description: ICM \_ -сообщение get получает значение DWORD, определенное приложением, из драйвера сжатия видео.
ms.assetid: 288c0053-16a1-4547-b748-da218a0b588c
keywords:
- сообщение ICM_GET Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_GET
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e23cd994546be41b5f938331b2dc632897635c32
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370581"
---
# <a name="icm_get-message"></a>ICM \_ Get, сообщение

ICM-сообщение **\_ Get** получает значение **DWORD** , определенное приложением, из драйвера сжатия видео.


```C++
ICM_GET 
wParam = (DWORD) (LPVOID) pv; 
lParam = (DWORD) cb; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="pv"></span><span id="PV"></span>*PV*
</dt> <dd>

Указатель на блок памяти, который должен быть заполнен текущим состоянием. Можно также указать **значение NULL** , чтобы определить объем памяти, необходимый для сведений о состоянии.

</dd> <dt>

<span id="cb"></span><span id="CB"></span>*CB*
</dt> <dd>

Размер блока памяти в байтах.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает объем памяти в байтах, необходимый для хранения сведений о состоянии.

## <a name="remarks"></a>Remarks

Структура, используемая для представления сведений о состоянии, зависит от драйвера и определяется драйвером.

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

 

 





