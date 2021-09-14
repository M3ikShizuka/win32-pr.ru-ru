---
title: Метод Адддиректконнектлиценсесервер класса Win32_TerminalServiceSetting
description: Адддиректконнектлиценсесервер больше не доступен.
ms.assetid: 7920fd28-0fa3-4f96-bec3-d9e37c97920c
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Адддиректконнектлиценсесервер
- Службы удаленных рабочих столов метода Адддиректконнектлиценсесервер, класс Win32_TerminalServiceSetting
- Класс Win32_TerminalServiceSetting службы удаленных рабочих столов, метод Адддиректконнектлиценсесервер
topic_type:
- apiref
api_name:
- Win32_TerminalServiceSetting.AddDirectConnectLicenseServer
api_location:
- TSCfgWmi.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: be9bba23f5c0bfc69b4c8d7951ab38eac6690b84
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967982"
---
# <a name="adddirectconnectlicenseserver-method-of-the-win32_terminalservicesetting-class"></a>Метод Адддиректконнектлиценсесервер \_ класса Win32 терминалсервицесеттинг

\[**адддиректконнектлиценсесервер** больше не доступен для использования в Windows Server 2008 R2.\]

**Windows Server 2008:** Настраивает новый сервер лицензирования и добавляет сервер лицензирования в реестр для обнаружения с помощью удаленный рабочий стол серверов узла сеансов удаленных рабочих столов.

## <a name="syntax"></a>Синтаксис


```mof
uint32 AddDirectConnectLicenseServer(
  [in] string LicenseServerName
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Лиценсесервернаме* \[ окне\]
</dt> <dd>

Имя добавляемого сервера лицензирования.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение 0 при успешном выполнении, в противном случае возвращает код ошибки WMI. Список этих значений см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md) .

## <a name="remarks"></a>Комментарии

файлы MOF-файл (MOF) содержат определения для классов инструментарий управления Windows (WMI) (WMI). файлы MOF не устанавливаются в составе пакета средств разработки программного обеспечения Microsoft Windows Software Development Kit (SDK). Они устанавливаются на сервере при добавлении связанной роли с помощью диспетчер сервера. Дополнительные сведения о файлах MOF см. в разделе [MOF-файл (MOF)](/windows/desktop/WmiSdk/managed-object-format--mof-).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                               |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Окончание поддержки клиента<br/>    | Ни одна версия не поддерживается<br/>                                                               |
| Поддержка конца сервера<br/>    | Windows Server 2008<br/>                                                          |
| Пространство имен<br/>                | Корневой \\ CIMv2 \\ терминалсервицес<br/>                                                |
| MOF<br/>                      | <dl> <dt>Тскфгвми. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>TSCfgWmi.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Терминалсервицесеттинг Win32**](win32-terminalservicesetting.md)
</dt> </dl>

 

