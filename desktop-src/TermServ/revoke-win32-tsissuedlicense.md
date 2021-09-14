---
title: Метод Revoke класса Win32_TSIssuedLicense
description: Отменяет лицензию на клиентский доступ службы удаленных рабочих столов на устройство (RDS \ 160; CAL "на устройство"), представленные \_ объектом Win32 тсиссуедлиценсе. Это не статическая функция.
ms.assetid: b1eb7448-5d8e-4c2d-ba52-9363e8e0297a
ms.tgt_platform: multiple
keywords:
- Отозвать метод службы удаленных рабочих столов
- Метод Revoke службы удаленных рабочих столов, Win32_TSIssuedLicense класс
- Win32_TSIssuedLicense класс службы удаленных рабочих столов, метод REVOKE
topic_type:
- apiref
api_name:
- Win32_TSIssuedLicense.Revoke
api_location:
- TlsWmiProv.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 63993ede5346f5b3cb56fcfa458d4cdce7dd58b8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127374544"
---
# <a name="revoke-method-of-the-win32_tsissuedlicense-class"></a>Метод Revoke \_ класса Win32 тсиссуедлиценсе

Отменяет клиентские лицензии службы удаленных рабочих столов на устройство (CAL для устройств RDS), представленные объектом [**Win32 \_ тсиссуедлиценсе**](win32-tsissuedlicense.md) . Это не статическая функция.

## <a name="syntax"></a>Синтаксис


```mof
uint32 Revoke(
  [out] uint32   RevokableCals,
  [out] DATETIME NextRevokeAllowedOn
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Ревокаблекалс* \[ заполняет\]
</dt> <dd>

Количество клиентских лицензий служб удаленных рабочих столов того же типа, что и текущий объект, который можно отозвать.

</dd> <dt>

*Некстревокеалловедон* \[ заполняет\]
</dt> <dd>

Дата, с которой администратор может далее попытаться отозвать лицензии. Этот параметр содержит только допустимые данные, если не удалось вызвать метод **REVOKE** , так как достигнуто максимальное число отмен.

</dd> </dl>

## <a name="remarks"></a>Remarks

Для вызова этого метода необходимо быть членом группы администраторов.

Можно отозвать только клиентские лицензии RDS "на устройство".

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

[**\_Тсиссуедлиценсе Win32**](win32-tsissuedlicense.md)
</dt> </dl>

 

