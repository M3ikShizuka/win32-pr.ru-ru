---
title: IDXCoreAdapterFactory::IsNotificationTypeSupported
description: Определяет, поддерживается ли указанный тип уведомлений операционной системой (ОС).
ms.localizationpriority: low
ms.topic: reference
ms.date: 06/20/2019
ms.openlocfilehash: 78730167e7ec139733ee1e4011d2e5e59c32782b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126966341"
---
# <a name="idxcoreadapterfactoryisnotificationtypesupported-method"></a>Метод Идкскореадаптерфактори:: Иснотификатионтипесуппортед

Определяет, поддерживается ли указанный тип уведомлений операционной системой (ОС). Инструкции по программированию и примеры кода см. [в разделе Использование дкскоре для перечисления адаптеров](../dxcore-enum-adapters.md).

## <a name="syntax"></a>Синтаксис

```cpp
virtual bool STDMETHODCALLTYPE IsNotificationTypeSupported(
  DXCoreNotificationType notificationType) = 0;
```

## <a name="parameters"></a>Параметры

### <a name="notificationtype"></a>notificationType

Тип: **[дкскоренотификатионтипе](./ne-dxcore_interface-dxcorenotificationtype.md)**

Тип уведомления, для которого запрашиваются сведения о поддержке. Сведения о типах уведомлений см. в таблице в [дкскоренотификатионтипе](./ne-dxcore_interface-dxcorenotificationtype.md) .

## <a name="returns"></a>Возвращаемое значение

Тип: **bool** .

Возвращает значение, `true` Если тип уведомления поддерживается системой. В противном случае возвращается `false`.

## <a name="remarks"></a>Комментарии

Можно вызвать **иснотификатионтипесуппортед** , чтобы определить, известен ли данный тип уведомления данной версии операционной системы. например, тип уведомления, представленный в определенной версии Windows, неизвестен предыдущим версиям Windows.

## <a name="see-also"></a>См. также раздел

[Идкскореадаптерфактори](./nn-dxcore_interface-idxcoreadapterfactory.md), [ДКСКОРЕ Reference](../dxcore-reference.md), [GUID атрибутов адаптера дкскоре](../dxcore-adapter-attribute-guids.md), [Использование дкскоре для перечисления адаптеров](../dxcore-enum-adapters.md)