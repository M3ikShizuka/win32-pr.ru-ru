---
description: Доставка конца потока
ms.assetid: 23afdb2e-93b0-4a74-94bd-e38eb82a5995
title: Доставка конца потока
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e2bd80d186bd62e6360fa1600f4ba970281315aa
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053486"
---
# <a name="delivering-the-end-of-stream"></a>Доставка конца потока

Когда входной ПИН-код получает уведомление об окончании потока, он распространяет вызов в нисходящем направлении. Все нисходящие фильтры, получающие данные из этого ПИН-кода, также должны получать уведомление об окончании потока. Опять же, переведите блокировку потоковой передачи, а не блокировку фильтра. Если фильтр содержит незавершенные данные, которые еще не были доставлены, то перед отправкой уведомления об окончании потока фильтр должен доставлять его. Он не должен передавать данные после конца потока.


```C++
HRESULT CMyInputPin::EndOfStream()
{
    CAutoLock lock_it(&m_csReceive);

    /* If the pin has not delivered all of the data in the stream 
       (based on what it received previously), do so now.  */

    // Propagate EndOfStream call downstream, via your output pin(s).
    for (each output pin)
    {    
        hr = pOutputPin->DeliverEndOfStream();
    }
    return S_OK;
}
```



Метод [**кбасеаутпутпин::D еливерендофстреам**](cbaseoutputpin-deliverendofstream.md) вызывает [**Ипин:: EndOfStream**](/windows/desktop/api/Strmif/nf-strmif-ipin-endofstream) на нисходящем входном закрепление.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Потоки и критические разделы](threads-and-critical-sections.md)
</dt> </dl>

 

 



