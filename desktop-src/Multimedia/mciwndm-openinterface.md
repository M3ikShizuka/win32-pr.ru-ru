---
title: Сообщение MCIWNDM_OPENINTERFACE (VFW. h)
description: Сообщение МЦИВНДМ \_ опенинтерфаце присоединяет поток данных или файл, связанный с указанным интерфейсом, к окну мЦивнд. Это сообщение можно отправить явно или с помощью макроса МЦивндопенинтерфаце.
ms.assetid: 73cbd637-d315-4b39-a978-2b72aed1f303
keywords:
- сообщение MCIWNDM_OPENINTERFACE Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_OPENINTERFACE
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9c40453f4d587429508a5aae19bc432fc46088ae
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370716"
---
# <a name="mciwndm_openinterface-message"></a>\_Сообщение мЦивндм опенинтерфаце

Сообщение **мЦивндм \_ опенинтерфаце** присоединяет поток данных или файл, связанный с указанным интерфейсом, к окну мЦивнд. Это сообщение можно отправить явно или с помощью макроса [**мЦивндопенинтерфаце**](/windows/desktop/api/Vfw/nf-vfw-mciwndopeninterface) .


```C++
MCIWNDM_OPENINTERFACE 
wParam = 0; 
lParam = (LPARAM) (LPUNKNOWN) pUnk; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="pUnk"></span><span id="punk"></span><span id="PUNK"></span>*pUnk*
</dt> <dd>

Указатель на интерфейс ИАВИ, указывающий на файл или поток данных в файле.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает нуль в случае успеха или ошибку в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**мЦивндопенинтерфаце**](/windows/desktop/api/Vfw/nf-vfw-mciwndopeninterface)
</dt> </dl>

 

 





