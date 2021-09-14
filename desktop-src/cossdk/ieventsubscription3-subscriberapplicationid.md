---
description: Идентификатор GUID приложения подписчика.
ms.assetid: 46c91cae-ca31-4eac-baa8-d36910917f0f
title: 'Свойство IEventSubscription3:: Субскрибераппликатионид'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IEventSubscription3.SubscriberApplicationID
- IEventSubscription3.get_SubscriberApplicationID
- IEventSubscription3.put_SubscriberApplicationID
api_type:
- COM
api_location: ''
ms.openlocfilehash: c2e726d97821a7a7143f4971a4918227235adb9c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126888952"
---
# <a name="ieventsubscription3subscriberapplicationid-property"></a>Свойство IEventSubscription3:: Субскрибераппликатионид

Идентификатор GUID приложения подписчика.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_SubscriberApplicationID(
  [in]          BSTR bstrSubscriberApplicationID
);

HRESULT get_SubscriberApplicationID(
  [out, retval] BSTR *pbstrSubscriberApplicationID
);
```



## <a name="property-value"></a>Значение свойства

Строка, содержащая идентификатор GUID приложения подписчика.

## <a name="error-codes"></a>Коды ошибок

Этот метод может возвращать стандартные возвращаемые значения E \_ INVALIDARG, e \_ OUTOFMEMORY, e \_ непредвиденные, e \_ Fail и S \_ ОК.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/> |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>       |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**IEventSubscription3**](ieventsubscription3.md)
</dt> </dl>

 

 




