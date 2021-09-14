---
title: D2D1_TAG (D2d1. h)
description: Определяемое приложением 64-разрядное значение, используемое в параметре \ 160; пометить набор операций отрисовки.
ms.assetid: 4f363295-f140-4149-ba78-3abbc56eebe8
keywords:
- D2D1_TAG
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: aacd11aa016e64ed463f1809595c865ae7e1f124
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127163476"
---
# <a name="d2d1_tag"></a>\_Тег D2D1

Определяемое приложением 64-разрядное значение, используемое для пометки набора операций отрисовки.


```C++
typedef UINT64 D2D1_TAG;
```



## <a name="remarks"></a>Комментарии

Чтобы задать тег перед набором операций отрисовки, используйте метод [**ID2D1RenderTarget:: сеттагс**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-settags) . Чтобы получить текущий тег, используйте метод [**ID2D1RenderTarget:: Tags**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-gettags) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 7, Windows Vista с пакетом обновления 2 (SP2) и обновлением платформы для приложений для \[ классических приложений Windows Vista \|\]<br/>                          |
| Минимальная версия сервера<br/> | Windows сервер 2008 R2, Windows Server 2008 с пакетом обновления 2 (SP2) и обновлением платформы для Windows Server 2008 приложения \[ UWP для классических приложений \|\]<br/> |
| Минимальный поддерживаемый телефон<br/>  | Windows Phone 8,1 \[ Windows Phone Silverlight 8,1 и среда выполнения Windows приложения\]<br/>                                                  |
| Заголовок<br/>                   | <dl> <dt>D2d1. h</dt> </dl>                                                        |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**GetTags**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-gettags)
</dt> <dt>

[**сеттагс**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-settags)
</dt> </dl>

 

