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
ms.openlocfilehash: 251a645f0a4ceacdbfb4e2ab7e650f41e44dd508
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056816"
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



 

## <a name="remarks"></a>Комментарии

Это свойство объекта [**Counters**](counters.md) по умолчанию.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                            |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                  |
| DLL<br/>                      | <dl> <dt>Сисмон. ocx</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**каунтеритем**](counteritem.md)
</dt> <dt>

[**Counters**](counters.md)
</dt> </dl>

 

 





