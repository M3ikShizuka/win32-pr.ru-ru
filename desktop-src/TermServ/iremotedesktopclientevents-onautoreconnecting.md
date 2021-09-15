---
title: Иремотедесктопклиентевентс Онаутореконнектинг, метод
description: Вызывается, когда клиентский элемент управления пытается автоматически восстановить соединение с удаленным сеансом.
ms.assetid: 299408A9-ED14-42F4-B324-AF4C86FEDABE
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Онаутореконнектинг
- Службы удаленных рабочих столов метода Онаутореконнектинг, интерфейс Иремотедесктопклиентевентс
- Службы удаленных рабочих столов интерфейса Иремотедесктопклиентевентс, метод Онаутореконнектинг
topic_type:
- apiref
api_name:
- IRemoteDesktopClientEvents.OnAutoReconnecting
api_location:
- MsTscAx.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d74c37919384727fdf51aad004349478798a3ffd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127270483"
---
# <a name="iremotedesktopclienteventsonautoreconnecting-method"></a>Метод Иремотедесктопклиентевентс:: Онаутореконнектинг

Вызывается, когда клиентский элемент управления пытается автоматически восстановить соединение с удаленным сеансом.

## <a name="syntax"></a>Синтаксис


```C++
void OnAutoReconnecting(
  [in] long         disconnectReason,
  [in] long         ExtendedDisconnectReason,
  [in] BSTR         disconnectErrorMessage,
  [in] VARIANT_BOOL networkAvailable,
  [in] long         attemptCount,
  [in] long         maxAttemptCount
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*дисконнектреасон* \[ окне\]
</dt> <dd>

Причина события Disconnect.

</dd> <dt>

*Екстендеддисконнектреасон* \[ окне\]
</dt> <dd>

Расширенные сведения о событии Disconnect.

</dd> <dt>

*дисконнектеррормессаже* \[ окне\]
</dt> <dd>

Сообщение об ошибке для события Disconnect.

</dd> <dt>

*нетворкаваилабле* \[ окне\]
</dt> <dd>

Доступна ли сеть.

</dd> <dt>

*аттемпткаунт* \[ окне\]
</dt> <dd>

В этом случае это.

</dd> <dt>

*максаттемпткаунт* \[ окне\]
</dt> <dd>

Будет выполнено максимальное число попыток повторного подключения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8<br/>                                                                           |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                                 |
| Библиотека типов<br/>             | <dl> <dt>MsTscAx.dll</dt> </dl>         |
| DLL<br/>                      | <dl> <dt>MsTscAx.dll</dt> </dl>         |
| IID<br/>                      | ДИИД \_ иремотедесктопклиентевентс определяется как 079863B7-6D47-4105-8BFE-0CDCB360E67D<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**иремотедесктопклиентевентс**](iremotedesktopclientevents.md)
</dt> </dl>

 

 





