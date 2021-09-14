---
title: Сообщение MCIWNDM_GETFILENAME (VFW. h)
description: Сообщение МЦИВНДМ \_ . filename извлекает имя файла, которое в настоящее время используется устройством MCI. Это сообщение можно отправить явно или с помощью макроса МЦивнджетфиленаме.
ms.assetid: d61b1b6d-0fae-4732-993c-41e08a4e05be
keywords:
- сообщение MCIWNDM_GETFILENAME Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_GETFILENAME
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 232a1d829b5cdd6da23e7dd3fb0294b95ca79f4b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127375196"
---
# <a name="mciwndm_getfilename-message"></a>Сообщение МЦИВНДМ. \_ имя_файла

Сообщение **мЦивндм. \_ filename** извлекает имя файла, которое в настоящее время используется устройством MCI. Это сообщение можно отправить явно или с помощью макроса [**мЦивнджетфиленаме**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetfilename) .


```C++
MCIWNDM_GETFILENAME 
wParam = (WPARAM) (UINT) len; 
lParam = (LPARAM) (LPVOID) lp; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="len"></span><span id="LEN"></span>*len*
</dt> <dd>

Размер буфера в байтах.

</dd> <dt>

<span id="lp"></span><span id="LP"></span>*LP*
</dt> <dd>

Указатель на определенный приложением буфер для возврата имени файла.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает нуль в случае успеха или 1 в противном случае.

## <a name="remarks"></a>Remarks

Если строка с завершающим нулем, содержащая имя файла, длиннее, чем буфер, МЦивнд усекает имя файла.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мЦивнджетфиленаме**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetfilename)
</dt> </dl>

 

 





