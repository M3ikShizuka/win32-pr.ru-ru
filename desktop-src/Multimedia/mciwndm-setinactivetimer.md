---
title: Сообщение MCIWNDM_SETINACTIVETIMER (VFW. h)
description: Сообщение МЦИВНДМ \_ сетинактиветимер устанавливает период обновления, используемый мЦивнд для обновления TrackBar в окне мЦивнд, обновляет сведения о положении в строке заголовка окна и отправляет сообщения уведомления родительскому окну, когда окно мЦивнд неактивно. Это сообщение можно отправить явно или с помощью макроса МЦивндсетинактиветимер.
ms.assetid: 8900c372-0493-4a63-a027-ef6ecf8f8254
keywords:
- сообщение MCIWNDM_SETINACTIVETIMER Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_SETINACTIVETIMER
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ba4504d84b254dfb67616568f5f97bba8e3bc2e3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127250762"
---
# <a name="mciwndm_setinactivetimer-message"></a>\_Сообщение мЦивндм сетинактиветимер

Сообщение **мЦивндм \_ сетинактиветимер** устанавливает период обновления, используемый мЦивнд для обновления TrackBar в окне мЦивнд, обновляет сведения о положении в строке заголовка окна и отправляет сообщения уведомления родительскому окну, когда окно мЦивнд неактивно. Это сообщение можно отправить явно или с помощью макроса [**мЦивндсетинактиветимер**](/windows/desktop/api/Vfw/nf-vfw-mciwndsetinactivetimer) .


```C++
MCIWNDM_SETINACTIVETIMER 
wParam = (WPARAM) (UINT) inactive; 
lParam = 0; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="inactive"></span><span id="INACTIVE"></span>*Активный*
</dt> <dd>

Период обновления (в миллисекундах). Значение по умолчанию — 2000 миллисекунд.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение не возвращает значение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мЦивндсетинактиветимер**](/windows/desktop/api/Vfw/nf-vfw-mciwndsetinactivetimer)
</dt> </dl>

 

 





