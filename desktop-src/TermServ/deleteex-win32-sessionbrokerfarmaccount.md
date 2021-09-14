---
title: Метод Делетикс класса Win32_SessionBrokerFarmAccount
description: Класс Win32 \_ сессионброкерфармаккаунт больше не доступен для использования в Windows Server 2012. | Метод Делетикс класса Win32_SessionBrokerFarmAccount
ms.assetid: d30c5d3e-f63c-4b21-85ae-a0b8d5868d64
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Делетикс
- Службы удаленных рабочих столов метода Делетикс, класс Win32_SessionBrokerFarmAccount
- Класс Win32_SessionBrokerFarmAccount службы удаленных рабочих столов, метод Делетикс
topic_type:
- apiref
api_name:
- Win32_SessionBrokerFarmAccount.DeleteEx
api_location:
- TssdWmi.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: cdad7b1c7af85337ace59690bb44f4309254eb76
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126891229"
---
# <a name="deleteex-method-of-the-win32_sessionbrokerfarmaccount-class"></a>Метод Делетикс \_ класса Win32 сессионброкерфармаккаунт

\[Класс [**Win32 \_ сессионброкерфармаккаунт**](win32-sessionbrokerfarmaccount.md) больше не доступен для использования в Windows Server 2012.\]

Удаляет учетную запись фермы.

## <a name="syntax"></a>Синтаксис


```mof
uint32 DeleteEx(
  [in] boolean DeleteComputerObject
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Делетекомпутеробжект* \[ окне\]
</dt> <dd>

Указывает, следует ли удалять объект-компьютер, связанный с фермой, из Active Directory.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение 0 при успешном выполнении, в противном случае возвращает код ошибки WMI. Список этих значений см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                              |
| Минимальная версия сервера<br/> | Windows Server 2008 R2<br/>                                                      |
| Окончание поддержки клиента<br/>    | Ни одна версия не поддерживается<br/>                                                              |
| Поддержка конца сервера<br/>    | Windows Server 2008 R2<br/>                                                      |
| Пространство имен<br/>                | Корневой \\ CIMv2 \\ терминалсервицес<br/>                                               |
| MOF<br/>                      | <dl> <dt>Тссдвми. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>TssdWmi.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Сессионброкерфармаккаунт Win32**](win32-sessionbrokerfarmaccount.md)
</dt> </dl>

 

 





