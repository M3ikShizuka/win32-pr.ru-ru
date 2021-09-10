---
title: Сообщение WM_CAP_SET_USER_DATA (VFW. h)
description: '\_ \_ Сообщение пользовательских данных для установки крепления WM \_ \_ связывает длинное \_ значение PTR с окном записи. Это сообщение можно отправить явно или с помощью макроса Капсетусердата.'
ms.assetid: 067502e3-f009-4cf2-b612-4a0b64624416
keywords:
- сообщение WM_CAP_SET_USER_DATA Windows мультимедиа
topic_type:
- apiref
api_name:
- WM_CAP_SET_USER_DATA
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 542b8e49f740bfc265824947237841dede1f6065
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371451"
---
# <a name="wm_cap_set_user_data-message"></a>\_Сообщение о \_ задании \_ \_ данных пользователя с закреплениями WM

Сообщение **\_ \_ \_ пользовательских \_ данных для установки крепления WM** связывает **длинное значение \_ ptr** с окном записи. Это сообщение можно отправить явно или с помощью макроса [**капсетусердата**](/windows/desktop/api/Vfw/nf-vfw-capsetuserdata) .


```C++
WM_CAP_SET_USER_DATA 
wParam = (WPARAM) 0; 
lParam = (LPARAM)lUser; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="lUser"></span><span id="luser"></span><span id="LUSER"></span>*лусер*
</dt> <dd>

Значение типа данных, связываемое с окном записи.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** в случае успеха или **false** , если потоковая запись выполняется.

## <a name="remarks"></a>Remarks

Обычно это сообщение используется для указания на блок данных, связанных с окном записи.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Видеозапись](video-capture.md)
</dt> <dt>

[Сообщения видеозаписи](video-capture-messages.md)
</dt> </dl>

 

 





