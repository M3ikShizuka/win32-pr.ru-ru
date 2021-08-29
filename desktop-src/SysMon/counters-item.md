---
title: Свойство Counters. Item
description: Извлекает указанный экземпляр Каунтеритем из коллекции.
ms.assetid: bf503371-c8bd-4e0d-ab8d-58de3f8fac5f
keywords:
- Свойство элемента Сисмон
- Свойство Item Сисмон, класс Counters
- Счетчики класса Сисмон, свойство Item
topic_type:
- apiref
api_name:
- Counters.Item
api_location:
- Sysmon.ocx
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 451a6e43714a9ca5ee8e64bf48fdf80aa9e5a9d7b99db8f78f997eba9404e284
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118883412"
---
# <a name="countersitem-property"></a>Свойство Counters. Item

Извлекает указанный экземпляр [**каунтеритем**](counteritem.md) из коллекции.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```VB
Property Item( _
  ByVal index As Object _
) As CounterItem
```



## <a name="property-value"></a>Значение свойства

Экземпляр [**каунтеритем**](counteritem.md) , соответствующий указанному значению индекса.

## <a name="exceptions"></a>Исключения



| Тип исключения                                  | Условие                         |
|-------------------------------------------------|-----------------------------------|
| **System. Runtime. InteropServices. COMException** | Указан недопустимый индекс. |



 

## <a name="remarks"></a>Remarks

Это свойство объекта [**Counters**](counters.md) по умолчанию.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                            |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                  |
| DLL<br/>                      | <dl> <dt>Сисмон. ocx</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**каунтеритем**](counteritem.md)
</dt> <dt>

[**Counters**](counters.md)
</dt> </dl>

 

 





