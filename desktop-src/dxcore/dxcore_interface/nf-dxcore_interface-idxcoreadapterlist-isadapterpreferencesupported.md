---
title: IDXCoreAdapterList::IsAdapterPreferenceSupported
description: Определяет, понимается ли заданное значение [дкскореадаптерпреференце](./ne-dxcore_interface-dxcoreadapterpreference.md) операционной системой.
ms.localizationpriority: low
ms.topic: reference
ms.date: 09/03/2019
ms.openlocfilehash: 1678568eb17c0dd833c130e6184931c8896261e9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126966326"
---
# <a name="idxcoreadapterlistisadapterpreferencesupported-method"></a>Метод Идкскореадаптерлист:: Исадаптерпреференцесуппортед

## <a name="description"></a>Описание

Определяет, понимается ли указанное значение [дкскореадаптерпреференце](./ne-dxcore_interface-dxcoreadapterpreference.md) текущей операционной системой (ОС). Можно вызвать **исадаптерпреференцесуппортед** перед вызовом [Идкскореадаптерлист:: Sort](./nf-dxcore_interface-idxcoreadapterlist-sort.md).

## <a name="syntax"></a>Синтаксис

```cpp
bool IsAdapterPreferenceSupported(
  DXCoreAdapterPreference preference
);
```

## <a name="parameters"></a>Параметры

### <a name="preference"></a>preference

Тип: **[дкскореадаптерпреференце](./ne-dxcore_interface-dxcoreadapterpreference.md)**

Значение [дкскореадаптерпреференце](./ne-dxcore_interface-dxcoreadapterpreference.md) , которое будет проверяться на наличие поддержки операционной системы.

## <a name="returns"></a>Возвращаемое значение

Тип: **bool** .

Возвращает значение, `true` Если тип сортировки понимается текущей ОС. В противном случае возвращается `false`.

## <a name="see-also"></a>См. также раздел

[Идкскореадаптерлист](./nn-dxcore_interface-idxcoreadapterlist.md), [дкскоре Reference](../dxcore-reference.md), [Использование дкскоре для перечисления адаптеров](../dxcore-enum-adapters.md)