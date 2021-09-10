---
title: Сообщение MCIWNDM_NEW (VFW. h)
description: '\_Новое сообщение мЦивндм создает новый файл для текущего устройства MCI. Это сообщение можно отправить явно или с помощью макроса МЦивнднев.'
ms.assetid: 18b2340d-8303-415a-867f-bd346034db2a
keywords:
- сообщение MCIWNDM_NEW Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_NEW
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 293323cd0404da45e648024b35b7f96ef60fea61
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370695"
---
# <a name="mciwndm_new-message"></a>МЦИВНДМ \_ новое сообщение

**\_ Новое сообщение мЦивндм** создает новый файл для текущего устройства MCI. Это сообщение можно отправить явно или с помощью макроса [**мЦивнднев**](/windows/desktop/api/Vfw/nf-vfw-mciwndnew) .


```C++
MCIWNDM_NEW 
wParam = 0; 
lParam = (LPARAM) (LPVOID) lp; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="lp"></span><span id="LP"></span>*LP*
</dt> <dd>

Указатель на буфер, содержащий имя устройства MCI, которое будет использовать файл.

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

[**мЦивнднев**](/windows/desktop/api/Vfw/nf-vfw-mciwndnew)
</dt> </dl>

 

 





