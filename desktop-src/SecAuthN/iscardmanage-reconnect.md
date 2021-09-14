---
description: Позволяет приложению повторно подключаться к смарт-карте или модулю чтения без необходимости выдавать вызов отсоединения, за которым следует вызов Аттачбихандле или Аттачбифд соответственно.
ms.assetid: 450e817d-2cb2-4752-a86e-50cc8e434723
title: 'Метод Искардманаже:: Reconnect'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ISCardManage.Reconnect
api_type:
- COM
api_location: ''
ms.openlocfilehash: b8b05e6292a92267569eb1f53e10f6143554aba1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127244174"
---
# <a name="iscardmanagereconnect-method"></a>Метод Искардманаже:: Reconnect

\[Метод **Reconnect** доступен для использования в операционных системах, указанных в разделе требования. он недоступен для использования в Windows Server 2003 с пакетом обновления 1 (SP1) и более поздних версий, Windows Vista, Windows Server 2008 и последующих версиях операционной системы. [Модули смарт-карт](/previous-versions/windows/desktop/secsmart/smart-card-modules) предоставляют аналогичные функции.\]

Метод **Reconnect** позволяет приложению повторно подключаться к [*смарт-карте*](../secgloss/s-gly.md) или [*модулю чтения*](../secgloss/r-gly.md) без необходимости выдавать вызов [**отсоединения**](iscardmanage-detach.md) , за которым следует вызов [**аттачбихандле**](iscardmanage-attachbyhandle.md) или [**аттачбифд**](iscardmanage-attachbyifd.md) соответственно.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Reconnect();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает одно из следующих возможных значений:



| Код возврата                                                                                   | Описание                                  |
|-----------------------------------------------------------------------------------------------|----------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>          | Operation completed successfully (Операция выполнена успешно).<br/> |
| <dl> <dt>**E \_ OUTOFMEMORY**</dt> </dl> | Недостаточно памяти.<br/>                    |



 

## <a name="remarks"></a>Remarks

Чтобы подключить смарт-карту, вызовите [**аттачбихандле**](iscardmanage-attachbyhandle.md) или [**аттачбифд**](iscardmanage-attachbyifd.md).

Чтобы отключить смарт-карту, вызовите [**отсоединение**](iscardmanage-detach.md).

Список всех методов, определенных этим интерфейсом, см. в разделе [**искардманаже**](iscardmanage.md).

Кроме приведенных выше кодов ошибок COM, этот интерфейс может возвращать код ошибки смарт-карты, если для завершения запроса была вызвана функция смарт-карты. Дополнительные сведения см. в статье [возвращаемые значения смарт-карты](authentication-return-values.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/> |
| Окончание поддержки клиента<br/>    | Windows XP<br/>                                |
| Поддержка конца сервера<br/>    | Windows Server 2003<br/>                       |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**аттачбихандле**](iscardmanage-attachbyhandle.md)
</dt> <dt>

[**аттачбифд**](iscardmanage-attachbyifd.md)
</dt> <dt>

[**Соединил**](iscardmanage-detach.md)
</dt> <dt>

[**искардманаже**](iscardmanage.md)
</dt> </dl>

 

 
