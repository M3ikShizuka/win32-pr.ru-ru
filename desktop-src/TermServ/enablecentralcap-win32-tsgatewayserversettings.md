---
title: Метод Енаблецентралкап класса Win32_TSGatewayServerSettings
description: Управляет свойством Централкапенаблед, которое управляет политиками авторизации подключений службы удаленных рабочих столов (RD \ 160; CAP) для сервера шлюза удаленный рабочий стол (шлюз удаленных рабочих столов).
ms.assetid: 43e476df-714d-43bd-b40f-33511b7757a4
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Енаблецентралкап
- Службы удаленных рабочих столов метода Енаблецентралкап, класс Win32_TSGatewayServerSettings
- Класс Win32_TSGatewayServerSettings службы удаленных рабочих столов, метод Енаблецентралкап
topic_type:
- apiref
api_name:
- Win32_TSGatewayServerSettings.EnableCentralCAP
api_location:
- AagWmi.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 933e91a89f9a5afdcd2ae85fa6cb097ef0c29cd2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170632"
---
# <a name="enablecentralcap-method-of-the-win32_tsgatewayserversettings-class"></a>Метод Енаблецентралкап \_ класса Win32 тсгатевайсерверсеттингс

Управляет свойством **централкапенаблед** , которое управляет политиками авторизации подключений службы удаленных рабочих столов (RD CAP) для сервера шлюза удаленный рабочий стол (шлюза удаленных рабочих столов).

## <a name="syntax"></a>Синтаксис


```mof
uint32 EnableCentralCAP(
  [in] boolean CentralCAPEnabled
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Централкапенаблед* \[ окне\]
</dt> <dd>

Если задано **значение true**, будут использоваться RD CAP из центральных серверов Cap. Если задано значение **false**, будут использоваться только политики локального сервера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если метод завершается с ошибкой, он возвращает ноль. Если метод завершился неудачно, он возвращает ненулевое значение. Список кодов ошибок см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md).

## <a name="remarks"></a>Remarks

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

[**\_Тсгатевайсерверсеттингс Win32**](win32-tsgatewayserversettings.md)
</dt> </dl>

 

