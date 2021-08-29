---
description: Возвращает операцию приостановки приложения.
ms.assetid: 33FCAED5-7568-4483-A643-A536B53F7003
title: 'Свойство Исуспендинжевентаргс:: Суспендингоператион (Windows. ApplicationModel. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ISuspendingEventArgs.SuspendingOperation
- ISuspendingEventArgs.get_SuspendingOperation
- ISuspendingEventArgs.put_SuspendingOperation
api_type:
- COM
api_location:
- Windows.ApplicationModel.h
ms.openlocfilehash: a798f91c0fd9ec20da61685a29120106c0eaaa4804521bb5ec5f931291372c2e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120121554"
---
# <a name="isuspendingeventargssuspendingoperation-property"></a>Свойство Исуспендинжевентаргс:: Суспендингоператион

Возвращает операцию приостановки приложения.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_SuspendingOperation();

HRESULT get_SuspendingOperation(
  [out, retval] ISuspendingOperation **value
);
```



## <a name="property-value"></a>Значение свойства

Приостановка операции.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8<br/>                                                                                    |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                                          |
| Заголовок<br/>                   | <dl> <dt>Windows. ApplicationModel. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Windows. ApplicationModel. idl</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**исуспендинжевентаргс**](isuspendingeventargs.md)
</dt> </dl>

 

 




