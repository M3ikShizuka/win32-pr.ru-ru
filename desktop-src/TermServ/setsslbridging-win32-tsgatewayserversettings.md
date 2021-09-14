---
title: Метод Сетсслбридгинг класса Win32_TSGatewayServerSettings
description: Задает тип моста SSL, используемый сервером шлюза удаленный рабочий стол (шлюза удаленных рабочих столов).
ms.assetid: 11885b8b-491e-4d90-b4d4-f0a0fbe68cb1
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Сетсслбридгинг
- Службы удаленных рабочих столов метода Сетсслбридгинг, класс Win32_TSGatewayServerSettings
- Класс Win32_TSGatewayServerSettings службы удаленных рабочих столов, метод Сетсслбридгинг
topic_type:
- apiref
api_name:
- Win32_TSGatewayServerSettings.SetSslBridging
api_location:
- AagWmi.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 77181fb8d8661ec7ea7dc0ce70532281fb9c1bde
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127374424"
---
# <a name="setsslbridging-method-of-the-win32_tsgatewayserversettings-class"></a>Метод Сетсслбридгинг \_ класса Win32 тсгатевайсерверсеттингс

Задает тип моста SSL, используемый сервером шлюза удаленный рабочий стол (шлюза удаленных рабочих столов). Это значение хранится в свойстве **сслбридгинг** .

> [!IMPORTANT]
> При изменении типа моста SSL с помощью этого метода необходимо перезапустить службу шлюза удаленных рабочих столов, чтобы изменения вступили в силу.

 

## <a name="syntax"></a>Синтаксис


```mof
uint32 SetSslBridging(
  [in] uint32 SslBridging
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Сслбридгинг* \[ окне\]
</dt> <dd>

Тип: **UInt32**

Указывает новое значение моста SSL. Это может быть одно из следующих значений.

<dt>

0
</dt> <dd>

Мост SSL отсутствует.

</dd> <dt>

1
</dt> <dd>

Мост HTTPS для HTTP.

</dd> <dt>

2
</dt> <dd>

Мост HTTPS для HTTPS.

</dd> </dl> </dd> </dl>

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

 

