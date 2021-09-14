---
title: IDXCoreAdapter::IsSetStateSupported
description: Определяет, поддерживает ли этот объект адаптера Дкскоре и текущую операционную систему (ОС) установку значения указанного состояния адаптера.
ms.localizationpriority: low
ms.topic: reference
ms.date: 06/20/2019
ms.openlocfilehash: 284e38a622c882fce04278d9134908f55c9a25cb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126966365"
---
# <a name="idxcoreadapterissetstatesupported-method"></a>Метод Идкскореадаптер:: Иссетстатесуппортед

Определяет, поддерживает ли этот объект адаптера Дкскоре и текущую операционную систему (ОС) установку значения указанного состояния адаптера.

## <a name="syntax"></a>Синтаксис

```cpp
virtual bool STDMETHODCALLTYPE IsSetStateSupported( 
  DXCoreAdapterState property) = 0;
```

## <a name="parameters"></a>Параметры

### <a name="state"></a>state

Тип: **[дкскореадаптерстате](./ne-dxcore_interface-dxcoreadapterstate.md)**

Тип элемента состояния, для которого запрашиваются сведения о поддержке. Дополнительные сведения о каждом типе состояния адаптера см. в таблице в [дкскореадаптерстате](./ne-dxcore_interface-dxcoreadapterstate.md) .

## <a name="returns"></a>Возвращаемое значение

Тип: **bool** .

Возвращает `true` значение, если этот объект адаптера дкскоре и текущая операционная система (ОС) поддерживают задание указанного состояния адаптера. В противном случае возвращается `false`.

## <a name="see-also"></a>См. также раздел

[Идкскореадаптер](./nn-dxcore_interface-idxcoreadapter.md), [ДКСКОРЕ Reference](../dxcore-reference.md), [GUID атрибутов адаптера дкскоре](../dxcore-adapter-attribute-guids.md), [Использование дкскоре для перечисления адаптеров](../dxcore-enum-adapters.md)