---
title: Свойство Конфигид Ивмвиртуалмачине (Впккоминтерфацес. h)
description: Извлекает уникальный идентификатор виртуальной машины.
ms.assetid: e1679822-d733-4c7a-a5ad-82cbc24a6329
keywords:
- Конфигид свойство Virtual PC
- Конфигид свойство Virtual PC, интерфейс Ивмвиртуалмачине
- Ивмвиртуалмачине интерфейс Virtual PC, свойство Конфигид
topic_type:
- apiref
api_name:
- IVMVirtualMachine.ConfigID
- IVMVirtualMachine.get_ConfigID
api_location:
- VPCCOMInterfaces.h
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ea1cb17b63e41259ab721eab3503181402ab33c68a3070ee8e4707c97e24e610
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119768064"
---
# <a name="ivmvirtualmachineconfigid-property"></a>Свойство Ивмвиртуалмачине:: Конфигид

\[Windows Virtual PC больше не доступен для использования в Windows 8. Вместо этого используйте [поставщик WMI Hyper-V (v2)](/windows/desktop/HyperV_v2/windows-virtualization-portal).\]

Извлекает уникальный идентификатор виртуальной машины.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_ConfigID(
  [out, retval] BSTR *virtualMachineConfigID
);
```



## <a name="property-value"></a>Значение свойства

Уникальный идентификатор, идентифицирующий виртуальную машину.

## <a name="error-codes"></a>Коды ошибок



| Имя/значение                                                                                                                                                    | Значение                                      |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------|
| <dl> <dt>С \_ ОК</dt> <dt>0</dt> </dl>                       | Операция выполнена успешно.<br/>     |
| <dl> <dt>Д \_ </dt> <dt>0x80004003</dt> указателя </dl>         | Параметр имеет **значение NULL**.<br/>        |
| <dl> <dt>Виртуальная машина \_ \_Неизвестный \_ 0xA0040207 виртуальной машины</dt> <dt></dt> </dl> | Конфигурация неизвестна.<br/>     |
| <dl> <dt> \_ E \_ Exception</dt> <dt>0x80020009</dt> </dl> | Произошла непредвиденная ошибка.<br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                                    |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                     |
| Окончание поддержки клиента<br/>    | Windows 7<br/>                                                                          |
| Продукт<br/>                  | Windows Virtual PC<br/>                                                                 |
| Заголовок<br/>                   | <dl> <dt>Впккоминтерфацес. h</dt> </dl> |
| IID<br/>                      | IID \_ ивмвиртуалмачине определен как f7092aa1-33ed-4f78-a59f-c00adfc2edd7<br/>          |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ивмвиртуалмачине**](ivmvirtualmachine.md)
</dt> </dl>

 

