---
title: Сообщение MCIWNDM_SETTIMERS (VFW. h)
description: Сообщение МЦИВНДМ \_ сеттимерс задает периоды обновления, используемые мЦивнд для обновления TrackBar в окне мЦивнд, обновления сведений о положении, отображаемых в строке заголовка окна, и отправки сообщений уведомления родительскому окну.
ms.assetid: 06407c67-b620-4f80-9fe9-456cdf3d0666
keywords:
- сообщение MCIWNDM_SETTIMERS Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_SETTIMERS
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7bba3fa2e474a15dc23deb9cdc6d00d148b8cd3a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127250729"
---
# <a name="mciwndm_settimers-message"></a>\_Сообщение мЦивндм сеттимерс

Сообщение **мЦивндм \_ сеттимерс** задает периоды обновления, используемые мЦивнд для обновления TrackBar в окне мЦивнд, обновления сведений о положении, отображаемых в строке заголовка окна, и отправки сообщений уведомления родительскому окну. Это сообщение можно отправить явно или с помощью макроса [**мЦивндсеттимерс**](/windows/desktop/api/Vfw/nf-vfw-mciwndsettimers) .


```C++
MCIWNDM_SETTIMERS 
wParam = (WPARAM) (UINT) active; 
lParam = (LPARAM) (UINT) inactive; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="active"></span><span id="ACTIVE"></span>*Active*
</dt> <dd>

Период обновления, используемый МЦивнд, если это активное окно. Значение по умолчанию — 500 миллисекунд. служба хранилища для этого значения ограничено 16 битами.

</dd> <dt>

<span id="inactive"></span><span id="INACTIVE"></span>*Активный*
</dt> <dd>

Период обновления, используемый МЦивнд, если это неактивное окно. Значение по умолчанию — 2000 миллисекунд. служба хранилища для этого значения ограничено 16 битами.

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

[**мЦивндсеттимерс**](/windows/desktop/api/Vfw/nf-vfw-mciwndsettimers)
</dt> </dl>

 

 





