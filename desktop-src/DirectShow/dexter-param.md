---
description: Указывает значение, которое принимает свойство в определенный момент времени.
ms.assetid: 117868b7-65e5-4b3b-9e50-4106ee6a65d0
title: Структура DEXTER_PARAM (Кедит. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DEXTER_PARAM
api_type:
- HeaderDef
api_location:
- Qedit.h
ms.openlocfilehash: 22b0f6ef0a91f9a6d9163a03c17f6e86ee8b5f4e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065691"
---
# <a name="dexter_param-structure"></a>\_Структура param Декстер

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

Указывает значение, которое принимает свойство в определенный момент времени.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct {
  BSTR   Name;
  DISPID dispID;
  LONG   nValues;
} DEXTER_PARAM;
```



## <a name="members"></a>Участники

<dl> <dt>

**имя**;
</dt> <dd>

Имя свойства.

</dd> <dt>

**dispID**
</dt> <dd>

Зарезервировано. Задайте нулевое значение.

</dd> <dt>

**Значения**
</dt> <dd>

Количество значений, которые предполагает свойство.

</dd> </dl>

## <a name="remarks"></a>Remarks

Объект должен поддерживать интерфейс **IDispatch** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Кедит. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ипропертисеттер**](ipropertysetter.md)
</dt> <dt>

[**\_значение Декстер**](dexter-value.md)
</dt> </dl>

 

 




