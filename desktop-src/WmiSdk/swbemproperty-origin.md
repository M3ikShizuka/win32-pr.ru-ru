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
ms.openlocfilehash: f0aef6c1041e14d65ee3cbacaa40255421a1b064
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058381"
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

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Wbemdisp. h</dt> </dl>   |
| Библиотека типов<br/>             | <dl> <dt>Wbemdisp. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Wbemdisp.dll</dt> </dl> |
| CLSID<br/>                    | \_SWBEMPROPERTY CLSID<br/>                                                         |
| IID<br/>                      | IID \_ исвбемпроперти<br/>                                                          |



 

 




