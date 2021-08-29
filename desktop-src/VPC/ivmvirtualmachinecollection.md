---
title: Интерфейс Ивмвиртуалмачинеколлектион (Впккоминтерфацес. h)
description: определяет коллекцию виртуальных машин в Windows virtual PC. Чтобы получить объект Ивмвиртуалмачинеколлектион, используйте свойство VirtualMachines Ивмвиртуалпк.
ms.assetid: 3d34e791-2dba-4529-b489-96a0c6227294
keywords:
- Виртуальный ПК с интерфейсом Ивмвиртуалмачинеколлектион
- Ивмвиртуалмачинеколлектион интерфейс Virtual PC, описание
topic_type:
- apiref
api_name:
- IVMVirtualMachineCollection
api_location:
- VPCCOMInterfaces.h
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9d3ca6a04d95d20a6e18e5fe70b285becc6fb1744e1465dad4e20d0c28d9fa45
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120006794"
---
# <a name="ivmvirtualmachinecollection-interface"></a>Интерфейс Ивмвиртуалмачинеколлектион

\[Windows Virtual PC больше не доступен для использования в Windows 8. Вместо этого используйте [поставщик WMI Hyper-V (v2)](/windows/desktop/HyperV_v2/windows-virtualization-portal).\]

определяет коллекцию виртуальных машин в Windows virtual PC. Чтобы получить объект **ивмвиртуалмачинеколлектион** , используйте свойство [**Ивмвиртуалпк:: VirtualMachines**](ivmvirtualpc-virtualmachines.md) .

## <a name="members"></a>Элементы

Интерфейс **ивмвиртуалмачинеколлектион** наследует от интерфейса [**IDispatch**](/windows/win32/api/oaidl/nn-oaidl-idispatch) . **Ивмвиртуалмачинеколлектион** также имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Интерфейс **ивмвиртуалмачинеколлектион** имеет следующие свойства.



| Свойство                                                             | Тип доступа          | Описание                                                                    |
|:---------------------------------------------------------------------|:---------------------|:-------------------------------------------------------------------------------|
| [**\_NewEnum**](ivmvirtualmachinecollection--newenum.md)<br/> | Только для чтения<br/> | Перечислитель для коллекции.<br/>                                   |
| [**Count**](ivmvirtualmachinecollection-count.md)<br/>        | Только для чтения<br/> | Число виртуальных машин в этой коллекции.<br/>                  |
| [**Компонент**](ivmvirtualmachinecollection-item.md)<br/>          | Только для чтения<br/> | Объект виртуальной машины, соответствующий указанному индексу.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                                     |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                      |
| Окончание поддержки клиента<br/>    | Windows 7<br/>                                                                           |
| Продукт<br/>                  | Windows Virtual PC<br/>                                                                  |
| Заголовок<br/>                   | <dl> <dt>Впккоминтерфацес. h</dt> </dl>  |
| IID<br/>                      | IID \_ ивмвиртуалмачинеколлектион определен как 59f31786-2a3d-4fbf-9896-d85338ca0da1<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ивмвиртуалмачине**](ivmvirtualmachine.md)
</dt> <dt>

[**Ивмвиртуалпк:: VirtualMachines**](ivmvirtualpc-virtualmachines.md)
</dt> </dl>

 

