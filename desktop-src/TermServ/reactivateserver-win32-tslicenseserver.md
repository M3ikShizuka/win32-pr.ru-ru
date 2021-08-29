---
title: Метод Реактиватесервер класса Win32_TSLicenseServer
description: Повторно активирует сервер лицензий удаленный рабочий стол, используя новый идентификатор, полученный по телефону или через Интернет.
ms.assetid: dd9ff938-a683-4f60-b7cc-7580892953b6
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Реактиватесервер
- Службы удаленных рабочих столов метода Реактиватесервер, класс Win32_TSLicenseServer
- Класс Win32_TSLicenseServer службы удаленных рабочих столов, метод Реактиватесервер
topic_type:
- apiref
api_name:
- Win32_TSLicenseServer.ReactivateServer
api_location:
- TlsWmiProv.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: af8f9a886e40968cc5393512d29e7a90f3cfc8815725eea780abda8bd7872328
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119988804"
---
# <a name="reactivateserver-method-of-the-win32_tslicenseserver-class"></a>Метод Реактиватесервер \_ класса Win32 тслиценсесервер

Повторно активирует сервер лицензий удаленный рабочий стол, используя новый идентификатор, полученный по телефону или через Интернет.

## <a name="syntax"></a>Синтаксис


```mof
uint32 ReactivateServer(
  [in]  string sNewLicenseServerId,
  [out] uint32 ActivationStatus
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*сневлиценсесерверид* \[ окне\]
</dt> <dd>

Идентификатор сервера лицензирования удаленный рабочий стол, полученный по телефону или через Интернет.

</dd> <dt>

*ActivationStatus* \[ заполняет\]
</dt> <dd>

Возвращенное состояние активации может иметь одно из следующих значений.

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

Произошла неизвестная ошибка. Неизвестно, активирован ли сервер лицензий удаленный рабочий стол.

</dd> </dl> </dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если метод завершается с ошибкой, он возвращает ноль. Если метод завершился неудачно, он возвращает ненулевое значение. Список кодов ошибок см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md).

## <a name="remarks"></a>Remarks

Для вызова этого метода необходимо быть членом группы администраторов.

файлы MOF-файл (MOF) содержат определения для классов инструментарий управления Windows (WMI) (WMI). файлы MOF не устанавливаются в составе пакета средств разработки программного обеспечения Microsoft Windows Software Development Kit (SDK). Они устанавливаются на сервере при добавлении связанной роли с помощью диспетчер сервера. Дополнительные сведения о файлах MOF см. в разделе [MOF-файл (MOF)](/windows/desktop/WmiSdk/managed-object-format--mof-).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                 |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                            |
| Пространство имен<br/>                | Root\\CIMv2<br/>                                                                    |
| MOF<br/>                      | <dl> <dt>Тлсвмипров. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>TlsWmiProv.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_Тслиценсесервер Win32**](win32-tslicenseserver.md)
</dt> </dl>

 

