---
description: Свойство Origin объекта SWbemProperty извлекает имя класса WMI, в котором было введено это свойство. Для классов с иерархиями с глубоким наследованием часто желательно выяснить, какие свойства были объявлены в каких классах.
ms.assetid: 25bc0303-43b8-42da-a194-82213c1009d9
ms.tgt_platform: multiple
title: Свойство SWbemProperty. Origin (Wbemdisp. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SWbemProperty.Origin
- ISWbemProperty.Origin
- ISWbemProperty.get_Origin
api_type:
- COM
api_location:
- Wbemdisp.dll
ms.openlocfilehash: 3e072267a47ccbcd99ab05544672cf2c1456967cedf97283565a5d8a92aae655
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119898274"
---
# <a name="swbempropertyorigin-property"></a>SWbemProperty. Origin, свойство

Свойство **Origin** объекта [**SWbemProperty**](swbemproperty.md) извлекает имя класса WMI, в котором было введено это свойство. Для классов с иерархиями с глубоким наследованием часто желательно выяснить, какие свойства были объявлены в каких классах.

Если свойство является локальным (см [**. свбемкуалифиер. local**](swbemqualifier-islocal.md)), это значение совпадает с классом-владельцем. Это свойство доступно только для чтения.

Описание этого синтаксиса см. в разделе [соглашения о документе для API скриптов](document-conventions-for-the-scripting-api.md).

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```VB
SWbemProperty.Origin As String
```



## <a name="property-value"></a>Значение свойства

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Wbemdisp. h</dt> </dl>   |
| Библиотека типов<br/>             | <dl> <dt>Wbemdisp. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Wbemdisp.dll</dt> </dl> |
| CLSID<br/>                    | \_SWBEMPROPERTY CLSID<br/>                                                         |
| IID<br/>                      | IID \_ исвбемпроперти<br/>                                                          |



 

 




