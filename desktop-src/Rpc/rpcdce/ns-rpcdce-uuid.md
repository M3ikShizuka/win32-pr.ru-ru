---
title: UUID
description: Предоставляет уникальное обозначение объекта, такого как интерфейс, вектор точки входа диспетчера или объект клиента.
ms.localizationpriority: low
ms.topic: reference
ms.date: 09/09/2019
ms.openlocfilehash: 95d2d420502a5d92af64c902ffa82c709639d872
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127580186"
---
# <a name="uuid-structure"></a>Структура UUID

Структура **UUID** определяет универсальный уникальный идентификатор (UUID). **UUID** обеспечивает уникальное обозначение объекта, такого как интерфейс, вектор точки входа диспетчера или объект клиента.

Структура **UUID** является `typedef` синонимом для структуры [GUID](/windows/win32/api/guiddef/ns-guiddef-guid) .

## <a name="syntax"></a>Синтаксис

```cpp
typedef GUID UUID;
```

## <a name="remarks"></a>Remarks

Библиотеки времени выполнения RPC используют **UUID** s для проверки совместимости между клиентами и серверами, а также для выбора из нескольких реализаций интерфейса.

## <a name="requirements"></a>Требования

| &nbsp; | &nbsp; |
| ---- |:---- |
| **Header** | Определено в рпкдце. h; включить RPC. h |

## <a name="see-also"></a>См. также раздел

[Идентификатор GUID](/windows/win32/api/guiddef/ns-guiddef-guid) 
 [UUID \_ VECTOR (вектор](/windows/win32/api/rpcdce/ns-rpcdce-uuid_vector) )