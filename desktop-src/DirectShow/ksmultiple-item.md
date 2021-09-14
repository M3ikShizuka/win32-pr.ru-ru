---
description: '\_Структура элемента ксмултипле описывает размер и число свойств переменной длины в ПИН-кодах в режиме ядра.'
ms.assetid: aedbf7bc-393d-4ab5-afcd-d8822b925f07
title: Структура KSMULTIPLE_ITEM (KS. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- KSMULTIPLE_ITEM
api_type:
- HeaderDef
api_location:
- ks.h
ms.openlocfilehash: 62e26b1aa8804514588e66c1d02e1f0643e97bcb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053291"
---
# <a name="ksmultiple_item-structure"></a>\_Структура элемента ксмултипле

`KSMULTIPLE_ITEM`Структура описывает размер и число свойств переменной длины ПИН-кодов в режиме ядра.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct {
  ULONG Size;
  ULONG Count;
} KSMULTIPLE_ITEM, *PKSMULTIPLE_ITEM;
```



## <a name="members"></a>Участники

<dl> <dt>

**Размер**
</dt> <dd>

Размер возвращенного блока памяти в байтах. Размер включает структуру **\_ элемента ксмултипле** и элементы, которые следуют за ней.

</dd> <dt>

**Количество**
</dt> <dd>

Указывает общее число элементов, которые следуют за этой структурой.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|---------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>KS. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[DirectShow Сотрудник](directshow-structures.md)
</dt> <dt>

[**Икспин:: Кскуеримедиумс**](ikspin-ksquerymediums.md)
</dt> <dt>

[**регпинмедиум**](/windows/desktop/api/strmif/ns-strmif-regpinmedium)
</dt> </dl>

 

 




