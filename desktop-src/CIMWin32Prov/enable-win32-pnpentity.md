---
description: Включает это самонастраивающийся устройство.
ms.assetid: 8f2096c4-03b4-4005-9b97-0086f2b41080
ms.tgt_platform: multiple
title: Enable, метод класса Win32_PnPEntity
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Win32_PnPEntity.Enable
api_type:
- COM
api_location:
- CIMWin32.dll
ms.openlocfilehash: 8f64c833a29f4df3b353a7e9782ffea39396cece
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054963"
---
# <a name="enable-method-of-the-win32_pnpentity-class"></a>Enable, метод класса Win32 \_ пнпентити

Включает это самонастраивающийся устройство.

## <a name="syntax"></a>Синтаксис


```mof
Uint32 Enable(
  [out] boolean rebootNeeded
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ребутнидед* \[ заполняет\]
</dt> <dd>

Необходимость перезагрузки.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10 \[ только классические приложения\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Server 2016<br/>                                                          |
| Пространство имен<br/>                | Корневой \\ CIMV2<br/>                                                                  |
| MOF<br/>                      | <dl> <dt>Cimwin32. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Пнпентити Win32**](win32-pnpentity.md)
</dt> </dl>

 

 




