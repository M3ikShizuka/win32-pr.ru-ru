---
description: Сообщение ТСПИ LINE \_ сендмспдата отправляется, когда поставщику услуг телефонии (TSP) требуется передать сведения поставщику службы мультимедиа (MSP).
ms.assetid: 982f40b3-7758-493c-9d04-6480e3c9e86d
title: Сообщение LINE_SENDMSPDATA (Тспи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ce46664be0bc7f312af8b45cc5e06e13a7d91488
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127250030"
---
# <a name="line_sendmspdata-message"></a>Строка \_ сообщения сендмспдата

Сообщение ТСПИ **Line \_ сендмспдата** отправляется, когда поставщику услуг телефонии (TSP) требуется передать сведения поставщику службы мультимедиа (MSP).


```C++
            
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*хтлине* 
</dt> <dd>

Маркер TAPI для линии.

</dd> <dt>

*хткалл* 
</dt> <dd>

Маркер TAPI для вызова.

</dd> <dt>

*двмсг* 
</dt> <dd>

Строка значения \_ сендмспдата.

</dd> <dt>

*dwParam1* 
</dt> <dd>

Указывает MSP, который должен получить сообщение. Если значение равно 0, сообщение будет отправлено всем MSP. Это обработчик, который передается функции [**тспи \_ линекреатемспинстанце**](/windows/win32/api/tspi/nf-tspi-tspi_linecreatemspinstance) .

</dd> <dt>

*dwParam2* 
</dt> <dd>

Буфер для передачи в MSP. Этот буфер не интерпретируется интерфейсом TAPI.

</dd> <dt>

*dwParam3* 
</dt> <dd>

Размер (в байтах) буфера в *dwParam2*.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Чтобы это сообщение работало, поставщик услуг должен согласовать TAPI версии 3,0 или более поздней.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------|-----------------------------------------------------------------------------------|
| Версия TAPI<br/> | Требуется TAPI 2,2<br/>                                                      |
| Заголовок<br/>       | <dl> <dt>Тспи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Сведения о поставщике службы мультимедиа (MSP)](./about-the-media-service-provider-msp-.md)
</dt> <dt>

[**ТСПИ \_ линемспидентифи**](/windows/win32/api/tspi/nf-tspi-tspi_linemspidentify)
</dt> <dt>

[**ТСПИ \_ линекреатемспинстанце**](/windows/win32/api/tspi/nf-tspi-tspi_linecreatemspinstance)
</dt> <dt>

[**ТСПИ \_ линеклосемспинстанце**](/windows/win32/api/tspi/nf-tspi-tspi_lineclosemspinstance)
</dt> <dt>

[**ТСПИ \_ линереЦиевемспдата**](/windows/win32/api/tspi/nf-tspi-tspi_linereceivemspdata)
</dt> <dt>

[**линедевкапс**](/windows/win32/api/tapi/ns-tapi-linedevcaps)
</dt> </dl>

 

