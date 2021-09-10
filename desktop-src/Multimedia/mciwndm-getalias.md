---
title: Сообщение MCIWNDM_GETALIAS (VFW. h)
description: Сообщение МЦИВНДМ \_ . alias извлекает псевдоним, используемый для открытия устройства MCI или файла с помощью функции mciSendString. Это сообщение можно отправить явно или с помощью макроса МЦивнджеталиас.
ms.assetid: 37131b89-275c-4ab6-9278-0e08c42471bd
keywords:
- сообщение MCIWNDM_GETALIAS Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_GETALIAS
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9e971c50b9abc450387ac29f9a7331bfdca5c38c
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370632"
---
# <a name="mciwndm_getalias-message"></a>Сообщение МЦИВНДМ. \_ псевдоним

Сообщение **мЦивндм. \_ Alias** извлекает псевдоним, используемый для открытия устройства MCI или файла с помощью функции [**mciSendString**](/previous-versions//dd757161(v=vs.85)) . Это сообщение можно отправить явно или с помощью макроса [**мЦивнджеталиас**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetalias) .


```C++
MCIWNDM_GETALIAS 
wParam = 0; 
lParam = 0; 
```



## <a name="return-value"></a>Возвращаемое значение

Возвращает псевдоним устройства.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**mciSendString**](/previous-versions//dd757161(v=vs.85))
</dt> <dt>

[**мЦивнджеталиас**](/windows/desktop/api/Vfw/nf-vfw-mciwndgetalias)
</dt> </dl>

 

