---
title: Сообщение MCIWNDM_GETREPEAT (VFW. h)
description: Сообщение МЦИВНДМ \_ повторяемости определяет, активировано ли непрерывное воспроизведение. Это сообщение можно отправить явно или с помощью макроса МЦивнджетрепеат.
ms.assetid: 6d644117-e705-421f-b45f-9f0e833e6bc8
keywords:
- сообщение MCIWNDM_GETREPEAT Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_GETREPEAT
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ef47dc4f639c7aa34f7a00341e6ad2e19be909d1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057464"
---
# <a name="mciwndm_getrepeat-message"></a>\_Сообщение МЦИВНДМ Repeat

Сообщение **МЦИВНДМ \_ повторяемости** определяет, активировано ли непрерывное воспроизведение. Это сообщение можно отправить явно или с помощью макроса [**мЦивнджетрепеат**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetrepeat) .


```C++
MCIWNDM_GETREPEAT 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если непрерывное воспроизведение активировано, или **false** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**мЦивнджетрепеат**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetrepeat)
</dt> </dl>

 

 





