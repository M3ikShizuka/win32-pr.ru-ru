---
description: Разрешает потоку байтов HTTP Microsoft Media Foundation использовать моникеры URL-адресов (также называемые Urlmon).
ms.assetid: 8B7D2FF7-D8A8-49E9-8CED-D37853B97A8F
title: Свойство MFPKEY_HTTP_ByteStream_Enable_Urlmon (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1858f34a5f719caba1a48f049b95f2031b400240
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462056"
---
# <a name="mfpkey_http_bytestream_enable_urlmon-property"></a>МФПКЭЙ \_ HTTP \_ ByteStream \_ Enable \_ Urlmon, свойство

Разрешает потоку байтов HTTP Microsoft Media Foundation использовать моникеры URL-адресов (также называемые *Urlmon*).



Тип данных

Тип ПРОПВАРИАНТ (VT)

ПРОПВАРИАНТ, элемент

**VARIANT \_ bool**

Логическое значение VT \_

**булвал**



## <a name="remarks"></a>Remarks

Это свойство используется для настройки потока байтов HTTP Media Foundation. Чтобы задать свойство, передайте указатель [**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore) в сопоставитель источника. Дополнительные сведения см. [в разделе Настройка источника мультимедиа](configuring-a-media-source.md).

Если значение является **вариантным \_ true**, то поток байтов HTTP использует Urlmon для транспорта HTTP. В противном случае, если значение является **вариантным \_ false**, байтовый поток использует WinHTTP.

значение по умолчанию — **вариант \_ TRUE** для приложений магазина Windows и **вариант \_ FALSE** для Windows приложения для настольных систем.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> </dl>

 

 
