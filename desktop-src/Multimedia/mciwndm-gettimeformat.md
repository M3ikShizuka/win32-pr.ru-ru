---
title: Сообщение MCIWNDM_GETTIMEFORMAT (VFW. h)
description: Сообщение МЦИВНДМ \_ жеттимеформат извлекает текущий формат времени устройства MCI в двух формах как числовое значение и в виде строки. Это сообщение можно отправить явно или с помощью макроса МЦивнджеттимеформат.
ms.assetid: 01844872-5444-4f3b-92a3-64f80b94d3a0
keywords:
- сообщение MCIWNDM_GETTIMEFORMAT Windows мультимедиа
topic_type:
- apiref
api_name:
- MCIWNDM_GETTIMEFORMAT
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a09f969c009ff23bc0951ed2efbc0dbf7aa95dda
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057452"
---
# <a name="mciwndm_gettimeformat-message"></a>\_Сообщение мЦивндм жеттимеформат

Сообщение **мЦивндм \_ жеттимеформат** извлекает текущий формат времени устройства MCI в двух формах: как числовое значение и как строка. Это сообщение можно отправить явно или с помощью макроса [**мЦивнджеттимеформат**](/windows/desktop/api/Vfw/nf-vfw-mciwndgettimeformat) .


```C++
MCIWNDM_GETTIMEFORMAT 
wParam = (WPARAM) (UINT) len; 
lParam = (LPARAM) (LPSTR) lp; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="len"></span><span id="LEN"></span>*len*
</dt> <dd>

Размер буфера в байтах.

</dd> <dt>

<span id="lp"></span><span id="LP"></span>*LP*
</dt> <dd>

Указатель на буфер, содержащий строку формата времени, завершающуюся нулем.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает целое число, соответствующее константе MCI, определяющей формат времени.

## <a name="remarks"></a>Комментарии

Если длина строки формата времени превышает размер буфера возврата, МЦивнд усекает строку.

Устройство MCI может поддерживать один или несколько следующих форматов времени.



| Формат времени                      | Константа MCI               |
|----------------------------------|----------------------------|
| Байты                            | \_ \_ байты формата MCI         |
| Получен                           | \_кадры формата \_ MCI        |
| Часы, минуты, секунды          | \_Формат MCI \_ ХМс           |
| Миллисекунды                     | \_ \_ миллисекунды формата MCI  |
| Минуты, секунды, кадры         | формат MCI, \_ \_ MSF           |
| Примеры                          | \_примеры формата \_ MCI       |
| SMPTE 24                         | \_Формат MCI \_ SMPTE \_ 24     |
| SMPTE 25                         | \_Формат MCI \_ SMPTE \_ 25     |
| SMPTE 30                    | \_Формат MCI \_ SMPTE \_ 30DROP |
| SMPTE 30 (без перетаскивания)              | \_Формат MCI \_ SMPTE \_ 30     |
| Дорожек, минут, секунд, кадров | \_Формат MCI \_ тмсф          |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**мЦивнджеттимеформат**](/windows/desktop/api/Vfw/nf-vfw-mciwndgettimeformat)
</dt> </dl>

 

 





