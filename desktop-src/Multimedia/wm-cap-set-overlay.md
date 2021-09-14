---
title: Сообщение WM_CAP_SET_OVERLAY (VFW. h)
description: '\_ \_ \_ Сообщение наложения WM Cap Set включает или отключает режим наложения. В режиме наложения видео отображается с помощью наложения оборудования. Это сообщение можно отправить явно или с помощью макроса Каповерлай.'
ms.assetid: b74c0619-2b70-46e0-9acd-43d658529233
keywords:
- сообщение WM_CAP_SET_OVERLAY Windows мультимедиа
topic_type:
- apiref
api_name:
- WM_CAP_SET_OVERLAY
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f197ae3a7df9ad1520b84cf27fd15a1c76524ab1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127147314"
---
# <a name="wm_cap_set_overlay-message"></a>\_ \_ \_ Сообщение наложения WM Cap Set

Сообщение **\_ \_ \_ наложения WM Cap Set** включает или отключает режим наложения. В режиме наложения видео отображается с помощью наложения оборудования. Это сообщение можно отправить явно или с помощью макроса [**каповерлай**](/windows/desktop/api/Vfw/nf-vfw-capoverlay) .


```C++
WM_CAP_SET_OVERLAY 
wParam = (WPARAM) (BOOL) (f); 
lParam = 0L; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="f"></span><span id="F"></span>*ж*
</dt> <dd>

Флаг наложения. Укажите **true** для этого параметра, чтобы включить режим наложения, или **false** , чтобы отключить его.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** в случае успеха или **false** в противном случае.

## <a name="remarks"></a>Remarks

Использование оверлея не требует ресурсов ЦП.

Элемент **фхасоверлай** структуры [**капдриверкапс**](/windows/win32/api/vfw/ns-vfw-capdrivercaps) указывает, поддерживает ли устройство наложение. Элемент **фоверлайвиндов** структуры [**капстатус**](/windows/win32/api/vfw/ns-vfw-capstatus) указывает, включен ли режим оверлея в данный момент.

Включение режима наложения автоматически отключает режим предварительного просмотра.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Видеозапись](video-capture.md)
</dt> <dt>

[Сообщения видеозаписи](video-capture-messages.md)
</dt> </dl>

 

 





