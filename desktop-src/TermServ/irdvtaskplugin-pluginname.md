---
title: Свойство PluginName Ирдвтаскплугин (Тспубплугинком. h)
description: Содержит отображаемое имя агента задач.
ms.assetid: 6f414270-e90b-4075-80fe-f918acbdd205
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов свойства PluginName
- Службы удаленных рабочих столов свойства PluginName, интерфейс Ирдвтаскплугин
- Службы удаленных рабочих столов интерфейса Ирдвтаскплугин, свойство PluginName
topic_type:
- apiref
api_name:
- IRDVTaskPlugin.PluginName
- IRDVTaskPlugin.get_PluginName
api_location:
- tspubplugincom.h
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0262472e37a8ff3e5b9bb153d2e94f4e52029b14
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168672"
---
# <a name="irdvtaskpluginpluginname-property"></a>Ирдвтаскплугин: свойство Лугиннаме:P

Содержит отображаемое имя агента задач. Это имя используется только в целях ведения журнала.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_PluginName(
  [out, retval] BSTR *pVal
);
```



## <a name="property-value"></a>Значение свойства

Отображаемое имя агента задачи.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 7 Корпоративная<br/>                                                             |
| Минимальная версия сервера<br/> | Windows Server 2008 R2<br/>                                                           |
| Заголовок<br/>                   | <dl> <dt>Тспубплугинком. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ирдвтаскплугин**](irdvtaskplugin.md)
</dt> </dl>

 

 





