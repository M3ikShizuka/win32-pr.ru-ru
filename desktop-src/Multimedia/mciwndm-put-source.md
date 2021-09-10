---
title: Сообщение MCIWNDM_PUT_SOURCE (VFW. h)
description: '\_ \_ Сообщение источника мЦивндм размещение переопределяет координаты исходного прямоугольника, используемого для обрезки изображений AVI в ходе воспроизведения. Это сообщение можно отправить явно или с помощью макроса МЦивндпутсаурце.'
ms.assetid: cff95139-0302-4db3-bf2e-559e75257e85
keywords:
- сообщение MCIWNDM_PUT_SOURCE Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_PUT_SOURCE
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5407f420b8def6dda9795e87eb68943c9373b143
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370731"
---
# <a name="mciwndm_put_source-message"></a>МЦИВНДМ \_ Размещение \_ исходного сообщения

Сообщение **\_ \_ источника мЦивндм размещение** переопределяет координаты исходного прямоугольника, используемого для обрезки изображений AVI в ходе воспроизведения. Это сообщение можно отправить явно или с помощью макроса [**мЦивндпутсаурце**](/windows/desktop/api/Vfw/nf-vfw-mciwndputsource) .


```C++
MCIWNDM_PUT_SOURCE 
wParam = 0; 
lParam = (LPARAM) (LPRECT) prc; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="prc"></span><span id="PRC"></span>*PRC*
</dt> <dd>

Указатель на структуру [Rect](/previous-versions//ms536136(v=vs.85)) , содержащую координаты исходного прямоугольника.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает нуль в случае успеха или ошибку в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



 

