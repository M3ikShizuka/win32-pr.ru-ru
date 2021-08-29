---
description: Запрашивает изменение состояния репликации отношения репликации виртуальной машины на указанное значение.
ms.assetid: 8EC78CCC-2997-4239-A20C-BA56F848ECB6
title: 'Метод Msvm_ComputerSystem:: Рекуестрепликатионстатечанжеекс'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Msvm_ComputerSystem.RequestReplicationStateChangeEx
api_type:
- COM
api_location:
- vmms.exe
ms.openlocfilehash: 865a49913f2de19d21496fac6efbf845e1f79b9f1512ae57892b54a7c28771c4
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119561584"
---
# <a name="msvm_computersystemrequestreplicationstatechangeex-method"></a>Мсвм \_ ComputerSystem:: рекуестрепликатионстатечанжеекс, метод

Запрашивает изменение состояния репликации отношения репликации виртуальной машины на указанное значение. Пока изменение состояния выполняется, свойство **ReplicationState** изменяется на значение параметра *RequestedState* . Этот метод поддерживается только для экземпляров класса [**\_ ComputerSystem мсвм**](msvm-computersystem.md) , представляющих виртуальную машину.

## <a name="syntax"></a>Синтаксис


```C++
uint32 RequestReplicationStateChangeEx(
  [in]  string              ReplicationRelationship,
  [in]  uint16              RequestedState,
  [out] CIM_ConcreteJob Job,
  [in]  datetime            TimeoutPeriod
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Репликатионрелатионшип* \[ окне\]
</dt> <dd>

Строковое представление внедренного экземпляра класса [**мсвм \_ репликатионрелатионшип**](msvm-replicationrelationship.md) , определяющего отношение репликации для запроса на изменение состояния. Это необязательный параметр. Если он не указан, запрос выполняется в отношении первичной репликации.

</dd> <dt>

*RequestedState* \[ окне\]
</dt> <dd>

Новое состояние репликации. Параметр должен иметь одно из следующих значений.

<dt>

<span id="Ready_to_start_initial_replication"></span><span id="ready_to_start_initial_replication"></span><span id="READY_TO_START_INITIAL_REPLICATION"></span>

<span id="Ready_to_start_initial_replication"></span><span id="ready_to_start_initial_replication"></span><span id="READY_TO_START_INITIAL_REPLICATION"></span>**Все готово для запуска начальной репликации** (1)


</dt> <dd>

Все готово для запуска начальной репликации.

</dd> <dt>

<span id="Waiting_to_complete_initial_replication"></span><span id="waiting_to_complete_initial_replication"></span><span id="WAITING_TO_COMPLETE_INITIAL_REPLICATION"></span>

<span id="Waiting_to_complete_initial_replication"></span><span id="waiting_to_complete_initial_replication"></span><span id="WAITING_TO_COMPLETE_INITIAL_REPLICATION"></span>**Ожидание завершения начальной репликации** (2)


</dt> <dd>

Ожидание завершения начальной репликации.

</dd> <dt>

<span id="Replicating"></span><span id="replicating"></span><span id="REPLICATING"></span>

<span id="Replicating"></span><span id="replicating"></span><span id="REPLICATING"></span>**Репликация** (3)


</dt> <dd>

репликация.

</dd> <dt>

<span id="Synced_replication_complete"></span><span id="synced_replication_complete"></span><span id="SYNCED_REPLICATION_COMPLETE"></span>

<span id="Synced_replication_complete"></span><span id="synced_replication_complete"></span><span id="SYNCED_REPLICATION_COMPLETE"></span>**Синхронизированная репликация завершена** (4)


</dt> <dd>

Синхронизированная репликация завершена.

</dd> <dt>

<span id="Suspend"></span><span id="suspend"></span><span id="SUSPEND"></span>

<span id="Suspend"></span><span id="suspend"></span><span id="SUSPEND"></span>**Приостановка** (7)


</dt> <dd>

Приостановить репликацию.

</dd> <dt>

<span id="Cancel_Resynchronize"></span><span id="cancel_resynchronize"></span><span id="CANCEL_RESYNCHRONIZE"></span>

<span id="Cancel_Resynchronize"></span><span id="cancel_resynchronize"></span><span id="CANCEL_RESYNCHRONIZE"></span>**Отменить повторную синхронизацию** (9)


</dt> <dd>

Отменить повторную синхронизацию.

</dd> </dl> </dd> <dt>

*Задание* \[ заполняет\]
</dt> <dd>

Необязательная ссылка на объект [**мсвм \_ конкретежоб**](msvm-concretejob.md) , который возвращается, если операция выполняется асинхронно. При наличии возвращаемой ссылки можно использовать для отслеживания хода выполнения и получения результата метода.

</dd> <dt>

*Тимеаутпериод* \[ окне\]
</dt> <dd>

Этот параметр не используется.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает одно из следующих значений.



| Возвращаемый код и значение                                                                                                                                                                | Описание                                                                                                                 |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------|
| <dl> <dt>**Завершено без ошибки**</dt> <dt>0</dt> </dl>                    | Success<br/>                                                                                                          |
| <dl> <dt>**Параметры метода проверены — задание запущено**</dt> <dt>4096</dt> </dl> | Переход является асинхронным.<br/>                                                                                  |
| <dl> <dt>**Сбой**</dt> <dt>32768</dt> </dl>                                 |                                                                                                                             |
| <dl> <dt>**Отказано в доступе**</dt> <dt>32769</dt> </dl>                          |                                                                                                                             |
| <dl> <dt>**Не поддерживается**</dt> <dt>32770</dt> </dl>                          |                                                                                                                             |
| <dl> <dt>**Состояние неизвестно**</dt> <dt>32771</dt> </dl>                      |                                                                                                                             |
| <dl> <dt>**Время ожидания**</dt> <dt>32772</dt> </dl>                                |                                                                                                                             |
| <dl> <dt>**Недопустимый параметр**</dt> <dt>32773</dt> </dl>                      | Значение, указанное в одном из параметров, не поддерживается.<br/>                                                   |
| <dl> <dt>**Система используется**</dt> <dt>32774</dt> </dl>                       |                                                                                                                             |
| <dl> <dt>**Недопустимое состояние для этой операции**</dt> <dt>32775</dt> </dl>       | Значение, указанное в параметре *RequestedState* , не поддерживается в текущем режиме репликации или состоянии.<br/> |
| <dl> <dt>**Недопустимый тип данных**</dt> <dt>32776</dt> </dl>                    |                                                                                                                             |
| <dl> <dt>**Система недоступна**</dt> <dt>32777</dt> </dl>                |                                                                                                                             |
| <dl> <dt>**Недостаточно памяти**</dt> <dt>32778</dt> </dl>                          |                                                                                                                             |
| <dl> <dt>**Файл не найден**</dt> <dt>32779</dt> </dl>                         |                                                                                                                             |



 

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                                            |
| Минимальная версия сервера<br/> | Windows Server 2016 \[ только классические приложения\]<br/>                                                    |
| Пространство имен<br/>                | \\\\Корневая \\ виртуализация \\ версии 2<br/>                                                                 |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Мсвм \_ ComputerSystem**](msvm-computersystem.md)
</dt> </dl>

 

 




