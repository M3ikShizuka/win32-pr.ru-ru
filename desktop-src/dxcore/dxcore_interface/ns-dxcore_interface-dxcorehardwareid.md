---
title: DXCoreHardwareID
description: Представляет компоненты идентификатора оборудования PnP для адаптера.
ms.localizationpriority: low
ms.topic: reference
ms.date: 06/20/2019
ms.openlocfilehash: 6882d9aa16bf72fb33f9a254a6434becb37f9cb8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126964598"
---
# <a name="dxcorehardwareid-structure"></a>Структура Дкскорехардвареид

Представляет компоненты идентификатора оборудования PnP для адаптера.

## <a name="syntax"></a>Синтаксис

```cpp
struct DXCoreHardwareID
{
  uint32_t vendorID;
  uint32_t deviceID;
  uint32_t subSysID;
  uint32_t revision;
};
```

## <a name="members"></a>Участники

### <a name="vendorid"></a>Поставщика

Тип: **uint32_t \***

Идентификатор PCI поставщика оборудования адаптера.

### <a name="deviceid"></a>deviceId

Тип: **uint32_t \***

Идентификатор PCI аппаратного устройства адаптера.

### <a name="subsysid"></a>субсисид

Тип: **uint32_t \***

Идентификатор PCI аппаратной подсистемы адаптера.

### <a name="revision"></a>revision

Тип: **uint32_t \***

Идентификатор PCI для номера редакции адаптера.

## <a name="see-also"></a>См. также раздел

[Дкскоре Reference](../dxcore-reference.md), [Использование дкскоре для перечисления адаптеров](../dxcore-enum-adapters.md)