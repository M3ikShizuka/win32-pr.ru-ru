---
title: Свойство адаптера Ивмвиртуалнетворк (Впккоминтерфацес. h)
description: Извлекает перечисляемую коллекцию сетевых адаптеров, подключенных к виртуальной сети.
ms.assetid: d5b95831-4642-441e-93e8-34e125087a43
keywords:
- Адаптера свойство Virtual PC
- Адаптера свойство Virtual PC, интерфейс Ивмвиртуалнетворк
- Ивмвиртуалнетворк интерфейс Virtual PC, свойство адаптера
topic_type:
- apiref
api_name:
- IVMVirtualNetwork.NetworkAdapters
- IVMVirtualNetwork.get_NetworkAdapters
api_location:
- VPCCOMInterfaces.h
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 76cbcf6a4c1f4aeb5f7c16d1e3a25a0081e664f0b3d71708fd85c6b457acb1b7
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118122634"
---
# <a name="ivmvirtualnetworknetworkadapters-property"></a>Свойство Ивмвиртуалнетворк:: адаптера

\[Windows Virtual PC больше не доступен для использования в Windows 8. Вместо этого используйте [поставщик WMI Hyper-V (v2)](/windows/desktop/HyperV_v2/windows-virtualization-portal).\]

Извлекает перечисляемую коллекцию сетевых адаптеров, подключенных к виртуальной сети.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_NetworkAdapters(
  [out, retval] IVMNetworkAdapterCollection **networkInterfaceCollection
);
```



## <a name="property-value"></a>Значение свойства

Новый [**ивмнетворкадаптерколлектион**](ivmnetworkadaptercollection.md) , содержащий виртуальные сетевые карты, подключенные к этой виртуальной сети.

## <a name="error-codes"></a>Коды ошибок



| Имя/значение                                                                                                                                                    | Значение                                      |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------|
| <dl> <dt>С \_ ОК</dt> <dt>0</dt> </dl>                       | Операция выполнена успешно.<br/>     |
| <dl> <dt>Д \_ </dt> <dt>0x80004003</dt> указателя </dl>         | Параметр имеет **значение NULL**.<br/>        |
| <dl> <dt> \_ E \_ Exception</dt> <dt>0x80020009</dt> </dl> | Произошла непредвиденная ошибка.<br/> |



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                                    |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                     |
| Окончание поддержки клиента<br/>    | Windows 7<br/>                                                                          |
| Продукт<br/>                  | Windows Virtual PC<br/>                                                                 |
| Заголовок<br/>                   | <dl> <dt>Впккоминтерфацес. h</dt> </dl> |
| IID<br/>                      | IID \_ ивмвиртуалнетворк определен как 431cb7a1-2469-4563-b94e-38b987adca63<br/>          |



## <a name="see-also"></a>См. также

<dl> <dt>

[**ивмвиртуалнетворк**](ivmvirtualnetwork.md)
</dt> </dl>

 

