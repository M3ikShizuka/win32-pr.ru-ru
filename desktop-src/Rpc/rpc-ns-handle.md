---
title: RPC_NS_HANDLE (Рпкнси. h)
description: Маркер NS для RPC типа данных \_ \_ определяет маркер службы Name-Service.
ms.assetid: d9c2a376-4972-4f16-aa8d-f0e43d5ddb8d
keywords:
- RPC_NS_HANDLE
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3e72ee694e08be1b30a75dc1f5b986619043d592
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461542"
---
# <a name="rpc_ns_handle"></a>\_маркер NS \_ RPC

**\_ \_ Маркер NS для RPC** типа данных определяет маркер службы Name-Service.


```C++
typedef void* RPC_NS_HANDLE;
```



## <a name="remarks"></a>Remarks

Маркер службы имени — это непрозрачная переменная, содержащая сведения, которые используются библиотекой времени выполнения RPC для возврата следующих данных RPC из базы данных Name-Service:

-   Дескрипторы привязки сервера
-   UUID ресурсов, предлагаемых элементами профиля сервера
-   Члены группы

Областью действия маркера имени службы является из процедуры "Begin" с помощью соответствующей процедуры "Done".

Приложения отвечают за управление параллелизмом для дескрипторов службы Name-Service в потоках.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                |
| Заголовок<br/>                   | <dl> <dt>Рпкнси. h (включение RPC. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**рпкнсбиндингимпортбегин**](/windows/desktop/api/Rpcnsi/nf-rpcnsi-rpcnsbindingimportbegina)
</dt> <dt>

[**рпкнсбиндингимпортдоне**](/windows/desktop/api/Rpcnsi/nf-rpcnsi-rpcnsbindingimportdone)
</dt> <dt>

[**рпкнсбиндингимпортнекст**](/windows/desktop/api/Rpcnsi/nf-rpcnsi-rpcnsbindingimportnext)
</dt> <dt>

[**рпкнсбиндинглукупбегин**](/windows/desktop/api/Rpcnsi/nf-rpcnsi-rpcnsbindinglookupbegina)
</dt> <dt>

[**рпкнсбиндинглукупдоне**](/windows/desktop/api/Rpcnsi/nf-rpcnsi-rpcnsbindinglookupdone)
</dt> <dt>

[**рпкнсбиндинглукупнекст**](/windows/desktop/api/Rpcnsi/nf-rpcnsi-rpcnsbindinglookupnext)
</dt> </dl>

 

 





