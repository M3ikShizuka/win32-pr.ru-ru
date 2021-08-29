---
description: Сведения о методе конструктора для Кженериклист. Кженериклист (Вкслист. h). Этот метод использует параметры "pName" и "Иитемс".
ms.assetid: 2258ecd6-7594-4ff8-961b-9e5e1ae9ff82
title: Конструктор Кженериклист. Кженериклист (Вкслист. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CGenericList.CGenericList
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 0885ecc91b35e9845703b7169f45fd6f7aa3d55aa10f57fc7ddc68ef7d42129e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119813994"
---
# <a name="cgenericlistcgenericlist-constructor-wxlisth---pname-iitems-parameters"></a>Конструктор Кженериклист. Кженериклист (Вкслист. h) — pName, параметры Иитемс

Метод конструктора.

## <a name="syntax"></a>Синтаксис


```C++
CGenericList(
   TCHAR *pName,
   INT   iItems,
   BOOL  bLock,
   BOOL  bAlert
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pName* 
</dt> <dd>

Указатель на имя списка.

</dd> <dt>

*иитемс* 
</dt> <dd>

Размер кэша узлов.

</dd> <dt>

*Блок* 
</dt> <dd>

Не используется.

</dd> <dt>

*балерт* 
</dt> <dd>

Не используется.

</dd> </dl>

## <a name="remarks"></a>Remarks

Для повышения эффективности `CGenericList` класс поддерживает кэш узлов списка. Если вы понимаете, сколько элементов будет храниться в списке, используйте эту версию конструктора.

## <a name="requirements"></a>Requirements (Требования)

| Требование | Значение |
|-|-|
| Заголовок | вкслист. h (включает Потоки. h) |
| Библиотека| Стрмбасе. lib (розничные сборки); Стрмбасд. lib (отладочные сборки) |

## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кженериклист**](cgenericlist.md)
</dt> </dl>

 

 




