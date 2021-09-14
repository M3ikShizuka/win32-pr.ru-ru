---
description: Происходит при начале получения данных ответа.
ms.assetid: 7245725b-40dd-4282-b681-f0b2c191db94
title: 'Событие Ивинхттпрекуестевентс:: Онреспонсестарт'
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7a299c535dd854bff07f2c24989096f7b9e49fc3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056284"
---
# <a name="iwinhttprequesteventsonresponsestart-event"></a>Событие Ивинхттпрекуестевентс:: Онреспонсестарт

Событие **онреспонсестарт** возникает при начале получения данных ответа.

## <a name="syntax"></a>Синтаксис


```C++
void OnResponseStart(
  [in] long Status,
  [in] BSTR ContentType
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Состояние* \[ окне\]
</dt> <dd>

Получает стандартный код состояния, возвращенный с данными ответа. Коды состояния определяются в [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt).

</dd> <dt>

*ContentType* \[ окне\]
</dt> <dd>

Указывает тип получаемого содержимого, например "text/html" или "image/gif".

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Комментарии

Чтобы это событие произошло, используйте [**Open**](iwinhttprequest-open.md) для отправки HTTP-соединения в асинхронном режиме и используйте [**Send**](iwinhttprequest-send.md) для отправки запроса данных на Интернет-сервер.

Это первое событие WinHTTP, возникающее после [**отправки**](iwinhttprequest-send.md).

> [!Note]  
> сведения о Windows XP и Windows 2000 см. в разделе [требования к времени выполнения](winhttp-start-page.md) на начальной странице WinHTTP.

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP, Windows 2000 Professional с SP3 \[ только для настольных приложений\]<br/>            |
| Минимальная версия сервера<br/> | Windows сервер 2003, Windows 2000 server с пакетом обновления 3 (SP3), \[ только классические приложения\]<br/>         |
| Распространяемые компоненты<br/>          | WinHTTP 5,0 и Internet Explorer 5,01 или более поздней версии в Windows XP и Windows 2000.<br/> |
| IDL<br/>                      | <dl> <dt>HttpRequest. idl</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**ивинхттпрекуестевентс**](iwinhttprequestevents-interface.md)
</dt> <dt>

[**WinHttpRequest**](winhttprequest.md)
</dt> <dt>

[Версии WinHTTP](winhttp-versions.md)
</dt> </dl>

 

 




