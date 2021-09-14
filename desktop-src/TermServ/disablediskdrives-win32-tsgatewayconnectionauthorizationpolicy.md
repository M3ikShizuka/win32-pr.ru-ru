---
title: Метод Дисабледискдривес класса Win32_TSGatewayConnectionAuthorizationPolicy
description: Задает свойство Дискдривесдисаблед.
ms.assetid: bdc4a923-bda7-464a-95eb-95231374ac93
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Дисабледискдривес
- Службы удаленных рабочих столов метода Дисабледискдривес, класс Win32_TSGatewayConnectionAuthorizationPolicy
- Класс Win32_TSGatewayConnectionAuthorizationPolicy службы удаленных рабочих столов, метод Дисабледискдривес
topic_type:
- apiref
api_name:
- Win32_TSGatewayConnectionAuthorizationPolicy.DisableDiskDrives
api_location:
- AagWmi.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 63938ccae6e93e23bd754c1d18ede0008fe92257
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126891168"
---
# <a name="disablediskdrives-method-of-the-win32_tsgatewayconnectionauthorizationpolicy-class"></a>Метод Дисабледискдривес \_ класса Win32 тсгатевайконнектионаусоризатионполици

Задает свойство **дискдривесдисаблед** . Если свойство **девицередиректионтипе** имеет значение 2, то свойство **дискдривесдисаблед** управляет перенаправлением дисковых дисков клиента для сеансов, установленных с помощью сервера шлюза удаленный рабочий стол (шлюза удаленных рабочих столов).

## <a name="syntax"></a>Синтаксис


```mof
uint32 DisableDiskDrives(
  [in] boolean Disabled
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Отключено* \[ окне\]
</dt> <dd>

Новое значение для свойства **дискдривесдисаблед** .

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

[**\_Тсгатевайконнектионаусоризатионполици Win32**](win32-tsgatewayconnectionauthorizationpolicy.md)
</dt> </dl>

 

