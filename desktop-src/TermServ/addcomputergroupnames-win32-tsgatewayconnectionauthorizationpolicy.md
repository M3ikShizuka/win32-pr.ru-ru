---
title: Метод Аддкомпутерграупнамес класса Win32_TSGatewayConnectionAuthorizationPolicy
description: Добавляет указанные имена групп компьютеров в свойство Компутерграупнамес.
ms.assetid: f0c440d6-0cc2-48b4-b656-65f12e652151
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Аддкомпутерграупнамес
- Службы удаленных рабочих столов метода Аддкомпутерграупнамес, класс Win32_TSGatewayConnectionAuthorizationPolicy
- Класс Win32_TSGatewayConnectionAuthorizationPolicy службы удаленных рабочих столов, метод Аддкомпутерграупнамес
topic_type:
- apiref
api_name:
- Win32_TSGatewayConnectionAuthorizationPolicy.AddComputerGroupNames
api_location:
- AagWmi.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 72647ef66b9e2eeaed824b3e77c404214786b615
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066837"
---
# <a name="addcomputergroupnames-method-of-the-win32_tsgatewayconnectionauthorizationpolicy-class"></a>Метод Аддкомпутерграупнамес \_ класса Win32 тсгатевайконнектионаусоризатионполици

Добавляет указанные имена групп компьютеров в свойство **компутерграупнамес** .

## <a name="syntax"></a>Синтаксис


```mof
uint32 AddComputerGroupNames(
  [in] string ComputerGroupNames
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Компутерграупнамес* \[ окне\]
</dt> <dd>

Разделенный точками с запятой список имен групп компьютеров, добавляемых в свойство **компутерграупнамес** . Имена групп компьютеров должны иметь формат *домена \\ компутерграупнаме*.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если метод завершается с ошибкой, он возвращает ноль. Если метод завершился неудачно, он возвращает ненулевое значение. Список кодов ошибок см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md).

## <a name="remarks"></a>Remarks

Если в параметре *компутерграупнамес* указано несколько имен групп компьютеров и одно из имен не может быть обработано, никакие имена не будут обработаны.

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

[**\_Тсгатевайконнектионаусоризатионполици Win32**](win32-tsgatewayconnectionauthorizationpolicy.md)
</dt> </dl>

 

