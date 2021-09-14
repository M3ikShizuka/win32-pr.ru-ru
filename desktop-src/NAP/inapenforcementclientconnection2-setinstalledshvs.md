---
title: Метод INapEnforcementClientConnection2 Сетинсталледшвс (Напенфорцементклиент. h)
description: Используется агентом NAP для установки на клиенте установленных средств проверки работоспособности системы (SHV).
ms.assetid: 38aa99b9-a15a-414d-91fc-128de8f5a654
keywords:
- Метод Сетинсталледшвс NAP
- Метод Сетинсталледшвс NAP, интерфейс INapEnforcementClientConnection2
- INapEnforcementClientConnection2 интерфейса NAP, метод Сетинсталледшвс
topic_type:
- apiref
api_name:
- INapEnforcementClientConnection2.SetInstalledShvs
api_location:
- qagent.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6651cd5248094f82d9faa1862492f82648e94125
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461747"
---
# <a name="inapenforcementclientconnection2setinstalledshvs-method"></a>Метод INapEnforcementClientConnection2:: Сетинсталледшвс

> [!Note]  
> Платформа защиты доступа к сети недоступна начиная с Windows 10

 

Метод **сетинсталледшвс** используется агентом NAP для установки на клиенте установленных средств проверки работоспособности системы (SHV).

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetInstalledShvs(
  [in] SystemHealthEntityCount count,
  [in] SystemHealthEntityId    *ids
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*количество* \[ окне\]
</dt> <dd>

Значение [системхеалсентитикаунт](nap-datatypes.md) , указывающее количество средств SHV для установки в *идентификаторах*.

</dd> <dt>

*идентификаторы* \[ окне\]
</dt> <dd>

Указатель на значение [системхеалсентитид](nap-datatypes.md) , содержащее список идентификаторов SHV для установки.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Также могут возвращаться другие коды ошибок, относящиеся к COM.



| Код возврата                                                                                  | Описание                                    |
|----------------------------------------------------------------------------------------------|------------------------------------------------|
| <dl> <dt>**С \_ ОК**</dt> </dl>        | Метод успешно выполнен.<br/>          |
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl> | Параметр *Count* равен 0 (нулю).<br/> |



 

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

 

 





