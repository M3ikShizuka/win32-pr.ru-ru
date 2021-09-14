---
title: Метод Update класса Win32_TSGatewayRADIUSServer
description: Обновляет текущий сервер протокол RADIUS (RADIUS).
ms.assetid: 38a15768-66eb-40d6-a079-16555f2bf96a
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода обновления
- Метод Update службы удаленных рабочих столов, класс Win32_TSGatewayRADIUSServer
- Класс Win32_TSGatewayRADIUSServer службы удаленных рабочих столов, метод Update
topic_type:
- apiref
api_name:
- Win32_TSGatewayRADIUSServer.Update
api_location:
- AagWmi.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: be4faf0c87e49a507ac300d7e8b32f218ed006ea
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126890880"
---
# <a name="update-method-of-the-win32_tsgatewayradiusserver-class"></a>Метод Update \_ класса Win32 тсгатевайрадиуссервер

Обновляет текущий сервер протокол RADIUS (RADIUS).

## <a name="syntax"></a>Синтаксис


```mof
uint32 Update(
  [in] string Name,
  [in] string SharedSecret
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Имя* \[ окне\]
</dt> <dd>

Имя сервера RADIUS.

</dd> <dt>

*SharedSecret* \[ окне\]
</dt> <dd>

Общий секрет для сервера RADIUS.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если метод завершается с ошибкой, он возвращает ноль. Если метод завершился неудачно, он возвращает ненулевое значение. Список кодов ошибок см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md).

## <a name="remarks"></a>Комментарии

Для вызова этого метода необходимо быть членом группы администраторов.

файлы MOF-файл (MOF) содержат определения для классов инструментарий управления Windows (WMI) (WMI). файлы MOF не устанавливаются в составе пакета средств разработки программного обеспечения Microsoft Windows Software Development Kit (SDK). Они устанавливаются на сервере при добавлении связанной роли с помощью диспетчер сервера. Дополнительные сведения о файлах MOF см. в разделе [MOF-файл (MOF)](/windows/desktop/WmiSdk/managed-object-format--mof-).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                           |
| Пространство имен<br/>                | Корневой \\ CIMv2 \\ терминалсервицес<br/>                                                 |
| MOF<br/>                      | <dl> <dt>TSGateway. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>AagWmi.dll</dt> </dl>    |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Тсгатевайрадиуссервер Win32**](win32-tsgatewayradiusserver.md)
</dt> </dl>

 

