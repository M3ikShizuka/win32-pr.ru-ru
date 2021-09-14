---
title: Метод Тсгремовеадминмсг класса Win32_TSGatewayServerSettings
description: Удаляет административное сообщение для сервера шлюза. | Метод Тсгремовеадминмсг класса Win32_TSGatewayServerSettings
ms.assetid: 36b157de-80ee-46f8-9803-5012cf1d6f5f
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Тсгремовеадминмсг
- Службы удаленных рабочих столов метода Тсгремовеадминмсг, класс Win32_TSGatewayServerSettings
- Класс Win32_TSGatewayServerSettings службы удаленных рабочих столов, метод Тсгремовеадминмсг
topic_type:
- apiref
api_name:
- Win32_TSGatewayServerSettings.TSGRemoveAdminMsg
api_location:
- AagWmi.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5ba9877b9e8704c92eb482876ab69107e116207b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170615"
---
# <a name="tsgremoveadminmsg-method-of-the-win32_tsgatewayserversettings-class"></a>Метод Тсгремовеадминмсг \_ класса Win32 тсгатевайсерверсеттингс

Удаляет административное сообщение для сервера шлюза.

## <a name="syntax"></a>Синтаксис


```mof
uint32 TSGRemoveAdminMsg();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Тип: **UInt32**

Если метод завершается с ошибкой, он возвращает ноль. Если метод завершился неудачно, он возвращает ненулевое значение. Список кодов ошибок см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md).

## <a name="remarks"></a>Remarks

Для вызова этого метода необходимо быть членом группы администраторов.

файлы MOF-файл (MOF) содержат определения для классов инструментарий управления Windows (WMI) (WMI). файлы MOF не устанавливаются в составе пакета средств разработки программного обеспечения Microsoft Windows Software Development Kit (SDK). Они устанавливаются на сервере при добавлении связанной роли с помощью диспетчер сервера. Дополнительные сведения о файлах MOF см. в разделе [MOF-файл (MOF)](/windows/desktop/WmiSdk/managed-object-format--mof-).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008 R2<br/>                                                        |
| Пространство имен<br/>                | Корневой \\ CIMv2 \\ терминалсервицес<br/>                                                 |
| MOF<br/>                      | <dl> <dt>TSGateway. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>AagWmi.dll</dt> </dl>    |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Тсгатевайсерверсеттингс Win32**](win32-tsgatewayserversettings.md)
</dt> </dl>

 

