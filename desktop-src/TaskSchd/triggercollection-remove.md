---
title: Тригжерколлектион. Remove, метод
description: Для сценариев удаляет указанный триггер из коллекции триггеров, используемых задачей.
ms.assetid: 30dccf16-2b4c-4776-9c19-f82ddd859d45
keywords:
- триггеры планировщик задач, удаление
- Удалить метод планировщик задач
- Метод Remove планировщик задач, объект Тригжерколлектион
- Планировщик задач объекта Тригжерколлектион, метод Remove
topic_type:
- apiref
api_name:
- TriggerCollection.Remove
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 401e84e57b28db9b08fd7e93e85fb7bc35f60647
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126891368"
---
# <a name="triggercollectionremove-method"></a>Тригжерколлектион. Remove, метод

Для сценариев удаляет указанный триггер из коллекции триггеров, используемых задачей.

## <a name="syntax"></a>Синтаксис


```VB
TriggerCollection.Remove( _
  ByVal index _
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*индекс* \[ окне\]
</dt> <dd>

Индекс удаляемого триггера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

При удалении элементов Обратите внимание, что индекс для первого элемента в коллекции равен 1, а индекс последнего элемента — значение свойства [**тригжерколлектион. Count**](triggercollection-count.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                    |
| Библиотека типов<br/>             | <dl> <dt>Тасксчд. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Taskschd.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





