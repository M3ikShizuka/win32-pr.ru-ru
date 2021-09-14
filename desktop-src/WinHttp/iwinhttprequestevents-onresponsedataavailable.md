---
description: Происходит при доступе к данным из ответа.
ms.assetid: 62d02e3b-466a-4d3d-994b-0a1ae12049e1
title: 'Событие Ивинхттпрекуестевентс:: Онреспонседатааваилабле'
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 41cb2fbc680b1f6739a66bb68565188c8a5d78b4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056292"
---
# <a name="iwinhttprequesteventsonresponsedataavailable-event"></a>Событие Ивинхттпрекуестевентс:: Онреспонседатааваилабле

Событие **онреспонседатааваилабле** возникает при доступе к данным из ответа.

## <a name="syntax"></a>Синтаксис


```C++
void OnResponseDataAvailable(
  [in] SAFEARRAY(unsigned char) *Data
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Данные* \[ окне\]
</dt> <dd>

отсчитываемый от нуля массив байтов, который получает данные ответа, полученные службами Microsoft Windows HTTP (WinHTTP) вплоть до момента возникновения этого события. Это **вариант** типа VT \_ array \| VT \_ UI1.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Комментарии

Поскольку данные находятся в байтах, их необходимо преобразовать в широкие символы при помещении в строку расширенных символов (Юникод).

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

 

 




