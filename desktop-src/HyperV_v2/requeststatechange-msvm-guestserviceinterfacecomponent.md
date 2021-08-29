---
description: Запрашивает изменение состояния компонента интерфейса гостевой службы на указанное значение.
ms.assetid: D9F7CD03-0D86-4005-A600-5CC7082A5047
title: 'Метод Msvm_GuestServiceInterfaceComponent:: RequestStateChange'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Msvm_GuestServiceInterfaceComponent.RequestStateChange
api_type:
- COM
api_location:
- vmms.exe
ms.openlocfilehash: 2b04859406a2600650caa1d822215291a84656d6909740008c2a87a9787f87a8
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119501014"
---
# <a name="msvm_guestserviceinterfacecomponentrequeststatechange-method"></a>Мсвм \_ гуестсервицеинтерфацекомпонент:: RequestStateChange, метод

Запрашивает изменение состояния компонента интерфейса гостевой службы на указанное значение.

## <a name="syntax"></a>Синтаксис


```C++
uint32 RequestStateChange(
  [in]  uint16              RequestedState,
  [out] CIM_ConcreteJob Job,
  [in]  datetime            TimeoutPeriod
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*RequestedState* \[ окне\]
</dt> <dd>

Тип: **UInt16**

Новое состояние. Сведения помещаются в свойство **RequestedState** экземпляра, если код возврата метода **RequestStateChange** равен 0 или 4096. Дополнительные сведения см. в описании свойств **EnabledState** и **RequestedState** для элемента. Это должно быть одно из следующих значений.

<dt>

<span id="Enabled"></span><span id="enabled"></span><span id="ENABLED"></span>

**Включено** (2)


</dt> <dd></dd> <dt>

<span id="Disabled"></span><span id="disabled"></span><span id="DISABLED"></span>

**Отключено** (3)


</dt> <dd></dd> <dt>

<span id="Shut_Down"></span><span id="shut_down"></span><span id="SHUT_DOWN"></span>

**Завершение работы** (4)


</dt> <dd></dd> <dt>

<span id="Offline"></span><span id="offline"></span><span id="OFFLINE"></span>

**Вне сети** (6)


</dt> <dd></dd> <dt>

<span id="Test"></span><span id="test"></span><span id="TEST"></span>

**Тест** (7)


</dt> <dd></dd> <dt>

<span id="Defer"></span><span id="defer"></span><span id="DEFER"></span>

**Отложить** (8)


</dt> <dd></dd> <dt>

<span id="Quiesce"></span><span id="quiesce"></span><span id="QUIESCE"></span>

**Замораживание** (9)


</dt> <dd></dd> <dt>

<span id="Reboot"></span><span id="reboot"></span><span id="REBOOT"></span>

**Перезагрузка** (10)


</dt> <dd></dd> <dt>

<span id="Reset"></span><span id="reset"></span><span id="RESET"></span>

**Сброс** (11)


</dt> <dd></dd> <dt>

<span id="DMTF_Reserved"></span><span id="dmtf_reserved"></span><span id="DMTF_RESERVED"></span>

**Зарезервировано DMTF** (..)


</dt> <dd></dd> <dt>

<span id="Vendor_Reserved"></span><span id="vendor_reserved"></span><span id="VENDOR_RESERVED"></span>

**Поставщик зарезервирован** (32768.. 65535)


</dt> <dd></dd> </dl> </dd> <dt>

*Задание* \[ заполняет\]
</dt> <dd>

Тип: **[ **CIM \_ конкретежоб**](/previous-versions//cc136808(v=vs.85))**

Необязательная ссылка на объект [**мсвм \_ конкретежоб**](msvm-concretejob.md) , который возвращается, если операция выполняется асинхронно. При наличии возвращаемой ссылки можно использовать для отслеживания хода выполнения и получения результата метода.

</dd> <dt>

*Тимеаутпериод* \[ окне\]
</dt> <dd>

Тип: **DateTime**

Период времени ожидания, указывающий максимальный период времени, в течение которого клиент ждет перехода в новое состояние. Для указания времени ожидания необходимо использовать формат интервала. Значение 0 или **null** указывает, что у клиента нет требований к времени для перехода. Если это свойство не содержит значений 0 или **null** и реализация не поддерживает этот параметр, должен возвращаться код возврата 4098 (**Использование параметра времени ожидания не поддерживается**).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **UInt32**

Этот метод возвращает одно из следующих значений.



| Возвращаемый код и значение                                                                                                                                                                       | Описание         |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------|
| <dl> <dt>**Завершено без ошибки**</dt> <dt>0</dt> </dl>                           | Успешно.<br/> |
| <dl> <dt>**Не поддерживается**</dt> <dt>1</dt> </dl>                                     |                     |
| <dl> <dt>**Неизвестная или Неуказанная ошибка**</dt> <dt>2</dt> </dl>                         |                     |
| <dl> <dt>**Не удается завершить в течение времени ожидания**</dt> <dt>3</dt> </dl>            |                     |
| <dl> <dt>**Сбой**</dt> <dt>4</dt> </dl>                                            |                     |
| <dl> <dt>**Недопустимый параметр**</dt> <dt>5</dt> </dl>                                 |                     |
| <dl> <dt>**Используется**</dt> <dt>6</dt> </dl>                                            |                     |
| <dl> <dt>**Зарезервировано DMTF**</dt> <dt>..</dt> </dl>                                    |                     |
| <dl> <dt>**Параметры метода проверены — переход запущен**</dt> <dt>4096</dt> </dl> |                     |
| <dl> <dt>**Недопустимая смена состояния**</dt> <dt>4097</dt> </dl>                       |                     |
| <dl> <dt>**Использование параметра времени ожидания не поддерживается**</dt> <dt>4098</dt> </dl>         |                     |
| <dl> <dt>**Занято**</dt> <dt>4099</dt> </dl>                                           |                     |
| <dl> <dt>**Метод зарезервирован**</dt> <dt>4100.. 32767</dt> </dl>                         |                     |
| <dl> <dt>**Независимый от поставщика**</dt> <dt>32768.65 535</dt> </dl>                        |                     |



 

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                                                 |
| Пространство имен<br/>                | \\\\Корневая \\ виртуализация \\ версии 2<br/>                                                                 |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Мсвм \_ гуестсервицеинтерфацекомпонент**](msvm-guestserviceinterfacecomponent.md)
</dt> </dl>

 

