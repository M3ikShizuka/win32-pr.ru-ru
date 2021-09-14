---
description: Происходит при завершении данных ответа.
ms.assetid: 0df2031e-826f-436e-a689-201fa8b5c38f
title: 'Событие Ивинхттпрекуестевентс:: Онреспонсефинишед'
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 19d3a596e23028cec0401a21a1ee866ef6e51d9d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056291"
---
# <a name="iwinhttprequesteventsonresponsefinished-event"></a>Событие Ивинхттпрекуестевентс:: Онреспонсефинишед

Событие **онреспонсефинишед** возникает при завершении данных ответа.

## <a name="syntax"></a>Синтаксис


```C++
void OnResponseFinished();
```



## <a name="parameters"></a>Параметры

У этого события нет параметров.

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Комментарии

Это событие сигнализирует о получении всех данных ответа, относящихся к последнему запросу. [**Онреспонседатааваилабле**](iwinhttprequestevents-onresponsedataavailable.md) не повторяется до следующего запроса.

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

 

 




