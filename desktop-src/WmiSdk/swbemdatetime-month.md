---
description: Возвращает или задает значение, представляющее компонент месяца для значения DateTime.
ms.assetid: 05818f0a-7e15-4ddd-a6a7-9d16ae82cd3c
ms.tgt_platform: multiple
title: Свойство SWbemDateTime. month (Wbemdisp. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SWbemDateTime.Month
- ISWbemDateTime.Month
- ISWbemDateTime.get_Month
- ISWbemDateTime.put_Month
api_type:
- COM
api_location:
- Wbemdisp.dll
ms.openlocfilehash: 73769d73cffc5b9731cfd55785e2fa087182b33b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126965265"
---
# <a name="swbemdatetimemonth-property"></a>SWbemDateTime. month, свойство

Свойство **Month** объекта [**SWbemDateTime**](swbemdatetime.md) Возвращает или задает значение, представляющее компонент месяца для значения DateTime. Число должно быть в диапазоне от 01 до 12 или возвращена ошибка **вбемвалуеаутофранже** .

Описание этого синтаксиса см. в разделе [соглашения о документе для API скриптов](document-conventions-for-the-scripting-api.md).

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```VB
SWbemDateTime.Month As Long
```



## <a name="property-value"></a>Значение свойства

## <a name="examples"></a>Примеры

Примеры использования объекта [**SWbemDateTime**](swbemdatetime.md) для преобразования значений [**DateTime**](datetime.md) CIM в формат **fileTime** или в формат **\_ даты VT** см. в разделе [задачи WMI: даты и время](wmi-tasks--dates-and-times.md). Описание формата **DateTime** в CIM см. в разделе [Формат даты и времени](date-and-time-format.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Wbemdisp. h</dt> </dl>   |
| Библиотека типов<br/>             | <dl> <dt>Wbemdisp. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Wbemdisp.dll</dt> </dl> |
| CLSID<br/>                    | \_SWBEMDATETIME CLSID<br/>                                                         |
| IID<br/>                      | IID \_ исвбемдатетиме<br/>                                                          |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**SWbemDateTime. МонсспеЦифиед**](swbemdatetime-monthspecified.md)
</dt> <dt>

[**SWbemDateTime**](swbemdatetime.md)
</dt> <dt>

[DATETIME](datetime.md)
</dt> </dl>

 

 




