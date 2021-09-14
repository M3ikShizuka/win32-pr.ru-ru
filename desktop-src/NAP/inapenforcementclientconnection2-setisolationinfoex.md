---
title: Метод INapEnforcementClientConnection2 Сетисолатионинфоекс (Напенфорцементклиент. h)
description: Используется Напажент для установки сведений о изоляции клиента.
ms.assetid: 1b1a41a1-73a6-4c81-8366-15d06c67e228
keywords:
- Метод Сетисолатионинфоекс NAP
- Метод Сетисолатионинфоекс NAP, интерфейс INapEnforcementClientConnection2
- INapEnforcementClientConnection2 интерфейса NAP, метод Сетисолатионинфоекс
topic_type:
- apiref
api_name:
- INapEnforcementClientConnection2.SetIsolationInfoEx
api_location:
- qagent.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 711b4bfd27c3bd92d48a78f4767f5ed452b2d4f5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461746"
---
# <a name="inapenforcementclientconnection2setisolationinfoex-method"></a>Метод INapEnforcementClientConnection2:: Сетисолатионинфоекс

> [!Note]  
> Платформа защиты доступа к сети недоступна начиная с Windows 10

 

Метод **INapEnforcementClientConnection2:: сетисолатионинфоекс** используется напажент для установки сведений о изоляции клиента.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetIsolationInfoEx(
  [in] const IsolationInfoEx *isolationInfo
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*исолатионинфо* \[ окне\]
</dt> <dd>

Указатель на структуру [**исолатионинфоекс**](/windows/win32/api/naptypes/ns-naptypes-isolationinfoex) , которая содержит состояние подключения клиента.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Также могут возвращаться другие коды ошибок, относящиеся к COM.



| Код возврата                                                                                     | Описание                                                        |
|-------------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
| <dl> <dt>**С \_ ОК**</dt> </dl>           | Операция успешно завершена.<br/>                                    |
| <dl> <dt>**Д \_ ACCESSDENIED**</dt> </dl> | Ошибка разрешений, доступ запрещен.<br/>                       |
| <dl> <dt>**Д \_ OUTOFMEMORY**</dt> </dl>  | Не удалось выполнить операцию из – за пределов системных ресурсов.<br/> |



 

## <a name="remarks"></a>Remarks

Эта информация задается Напажент после обработки [**сохреспонсе**](/windows/win32/api/naptypes/ns-naptypes-soh) и не может быть задана в принудительном применении.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                      |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                |
| Заголовок<br/>                   | <dl> <dt>Напенфорцементклиент. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Напенфорцементклиент. idl</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Qagent.dll</dt> </dl>               |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**INapEnforcementClientConnection2**](inapenforcementclientconnection2.md)
</dt> </dl>

 

 





