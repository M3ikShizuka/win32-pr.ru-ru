---
description: Задает число рабочих потоков, используемых видеодекодером.
ms.assetid: A1570BB5-62BC-46C0-B9C9-61F99AA13BBE
title: Свойство CODECAPI_AVDecNumWorkerThreads (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c5d7c57d1b4176ad65313a5583a70f9ba4f7427a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574975"
---
# <a name="codecapi_avdecnumworkerthreads-property"></a>КОДЕКАПИ \_ авдекнумворкерсреадс, свойство

Задает число рабочих потоков, используемых видеодекодером.

## <a name="data-type"></a>Тип данных

**Long** (**VT \_ I4**)

## <a name="property-guid"></a>GUID свойства

КОДЕКАПИ \_ авдекнумворкерсреадс

## <a name="remarks"></a>Комментарии

Если значение равно 1, декодер выбирает число потоков.

Для интерфейса [**икодекапи**](/windows/desktop/api/strmif/nn-strmif-icodecapi) задайте для этого свойства значение **Long** (**VT \_ I4**). Для интерфейса [**имфаттрибутес**](/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes) установите это свойство как **UINT32**, хотя значение подписывается.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ приложения UWP для классических приложений \|\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ приложения UWP для классических приложений \|\]<br/>                           |
| Заголовок<br/>                   | <dl> <dt>Кодекапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> <dt>

[**икодекапи**](/windows/desktop/api/strmif/nn-strmif-icodecapi)
</dt> </dl>

 

