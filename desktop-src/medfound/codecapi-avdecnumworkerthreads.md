---
description: Задает число рабочих потоков, используемых видеодекодером.
ms.assetid: A1570BB5-62BC-46C0-B9C9-61F99AA13BBE
title: Свойство CODECAPI_AVDecNumWorkerThreads (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e1a17584e9a6e3d6f8efcfcf129a89bc0f94cb2629c0f130549a73757c20368f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119035362"
---
# <a name="codecapi_avdecnumworkerthreads-property"></a>КОДЕКАПИ \_ авдекнумворкерсреадс, свойство

Задает число рабочих потоков, используемых видеодекодером.

## <a name="data-type"></a>Тип данных

**Long** (**VT \_ I4**)

## <a name="property-guid"></a>GUID свойства

КОДЕКАПИ \_ авдекнумворкерсреадс

## <a name="remarks"></a>Remarks

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

 

