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
ms.openlocfilehash: 59db02d69302127937a7203729de9cc8b98a58f4
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370710"
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

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



 

 





