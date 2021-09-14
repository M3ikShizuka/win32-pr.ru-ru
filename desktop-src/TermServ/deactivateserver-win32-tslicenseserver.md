---
title: Метод Деактиватесервер класса Win32_TSLicenseServer
description: Деактивирует сервер лицензий удаленный рабочий стол, используя код подтверждения, полученный по телефону.
ms.assetid: 84e069b7-9a4f-4843-b656-839f936ac727
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Деактиватесервер
- Службы удаленных рабочих столов метода Деактиватесервер, класс Win32_TSLicenseServer
- Класс Win32_TSLicenseServer службы удаленных рабочих столов, метод Деактиватесервер
topic_type:
- apiref
api_name:
- Win32_TSLicenseServer.DeactivateServer
api_location:
- TlsWmiProv.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 23b851a8d8049c9194bce163afc4b7bad5d4aa15
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066818"
---
# <a name="deactivateserver-method-of-the-win32_tslicenseserver-class"></a>Метод Деактиватесервер \_ класса Win32 тслиценсесервер

Деактивирует сервер лицензий удаленный рабочий стол, используя код подтверждения, полученный по телефону.

## <a name="syntax"></a>Синтаксис


```mof
uint32 DeactivateServer(
  [in]  string sConfirmCode,
  [out] uint32 ActivationStatus
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*сконфирмкоде* \[ окне\]
</dt> <dd>

Код подтверждения.

</dd> <dt>

*ActivationStatus* \[ заполняет\]
</dt> <dd>

Возвращенное состояние активации может быть одним из следующих.

<dt>

0
</dt> <dd>

Сервер лицензий удаленный рабочий стол активирован.

</dd> <dt>

1
</dt> <dd>

Сервер лицензирования удаленный рабочий стол не активирован.

</dd> <dt>

2
</dt> <dd>

Произошла неизвестная ошибка. Неизвестно, активирован ли сервер лицензий службы удаленных рабочих столов.

</dd> </dl> </dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если метод завершается с ошибкой, он возвращает ноль. Если метод завершился неудачно, он возвращает ненулевое значение. Список кодов ошибок см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md).

## <a name="remarks"></a>Remarks

Для вызова этого метода необходимо быть членом группы администраторов.

файлы MOF-файл (MOF) содержат определения для классов инструментарий управления Windows (WMI) (WMI). файлы MOF не устанавливаются в составе пакета средств разработки программного обеспечения Microsoft Windows Software Development Kit (SDK). Они устанавливаются на сервере при добавлении связанной роли с помощью диспетчер сервера. Дополнительные сведения о файлах MOF см. в разделе [MOF-файл (MOF)](/windows/desktop/WmiSdk/managed-object-format--mof-).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                 |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                            |
| Пространство имен<br/>                | Root\\CIMv2<br/>                                                                    |
| MOF<br/>                      | <dl> <dt>Тлсвмипров. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>TlsWmiProv.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Тслиценсесервер Win32**](win32-tslicenseserver.md)
</dt> </dl>

 

