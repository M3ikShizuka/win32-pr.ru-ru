---
title: Сообщение MCIWNDM_NOTIFYSIZE (VFW. h)
description: Сообщение МЦИВНДМ \_ нотифисизе уведомляет родительское окно приложения о том, что размер окна изменился.
ms.assetid: 76e1f663-bfc6-4d3c-9486-c8c7f79e4265
keywords:
- сообщение MCIWNDM_NOTIFYSIZE Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_NOTIFYSIZE
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6793aa6d0e0f3001a5c8c76b34ed6bbd1011ba17441fd709ee016d9d161a97b4
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119525384"
---
# <a name="mciwndm_notifysize-message"></a>\_Сообщение мЦивндм нотифисизе

Сообщение **мЦивндм \_ нотифисизе** уведомляет родительское окно приложения о том, что размер окна изменился.


```C++
MCIWNDM_NOTIFYSIZE 
wParam = (WPARAM) (HWND) hwnd; 
lParam = 0; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="hwnd"></span><span id="HWND"></span>*HWND*
</dt> <dd>

Обработайте окно МЦивнд.

</dd> </dl>

## <a name="remarks"></a>Remarks

Вы можете включить уведомления об изменениях в размере окна МЦивнд, указав \_ стиль окна мЦивндф нотифисизе.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



 

 





