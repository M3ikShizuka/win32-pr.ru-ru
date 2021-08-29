---
title: IMsRdpDeviceV2 Девицетекст, свойство
description: Содержит текст устройства.
ms.assetid: 2a67e8d4-2af3-4738-ade2-a79800aea4a1
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов свойства Девицетекст
- Службы удаленных рабочих столов свойства Девицетекст, интерфейс IMsRdpDeviceV2
- Службы удаленных рабочих столов интерфейса IMsRdpDeviceV2, свойство Девицетекст
topic_type:
- apiref
api_name:
- IMsRdpDeviceV2.DeviceText
- IMsRdpDeviceV2.get_DeviceText
api_location:
- MsTscAx.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8ed156a56215c859455cd16cb5d4ae0396eb24a0b62c8b9ae0ee6d5a43bd2ad3
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119138607"
---
# <a name="imsrdpdevicev2devicetext-property"></a>IMsRdpDeviceV2: свойство Евицетекст:D

Содержит текст устройства. это имя, которое Windows отображается пользователю.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_DeviceText(
  [out, retval] BSTR *pDeviceText
);
```



## <a name="property-value"></a>Значение свойства

Отображаемое имя устройства.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 7 с пакетом обновления 1 (SP1)<br/>                                                          |
| Минимальная версия сервера<br/> | Windows Server 2008 R2 с пакетом обновления 1 (SP1)<br/>                                             |
| Библиотека типов<br/>             | <dl> <dt>MsTscAx.dll</dt> </dl> |
| DLL<br/>                      | <dl> <dt>MsTscAx.dll</dt> </dl> |
| IID<br/>                      | IID \_ IMsRdpDeviceV2 определен как 5fb94466-7661-42a8-98b7-01904c11668f<br/>      |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**IMsRdpDeviceV2**](imsrdpdevicev2.md)
</dt> </dl>

 

 





