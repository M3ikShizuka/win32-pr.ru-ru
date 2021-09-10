---
title: Сообщение MCIWNDM_NOTIFYMEDIA (VFW. h)
description: Сообщение МЦИВНДМ \_ нотифимедиа уведомляет родительское окно приложения о том, что носитель был изменен.
ms.assetid: cc31502d-09a9-4580-9ff8-9c2be51c8e35
keywords:
- сообщение MCIWNDM_NOTIFYMEDIA Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_NOTIFYMEDIA
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7026bd984e1d79775aac52caad56c87be6e8098e
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370701"
---
# <a name="mciwndm_notifymedia-message"></a>\_Сообщение мЦивндм нотифимедиа

Сообщение **мЦивндм \_ нотифимедиа** уведомляет родительское окно приложения о том, что носитель был изменен.


```C++
MCIWNDM_NOTIFYMEDIA 
wParam = (WPARAM) (HWND) hwnd; 
lParam = (LPARAM) (LPSTR) lp; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="hwnd"></span><span id="HWND"></span>*HWND*
</dt> <dd>

Обработайте окно МЦивнд.

</dd> <dt>

<span id="lp"></span><span id="LP"></span>*LP*
</dt> <dd>

Указатель на строку с завершающим нулем, содержащую новое имя файла. Если носитель закрывается, он указывает пустую строку.

</dd> </dl>

## <a name="remarks"></a>Remarks

Вы можете включить уведомления об изменениях мультимедиа, указав \_ стиль окна мЦивндф нотифимедиа.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



 

 





