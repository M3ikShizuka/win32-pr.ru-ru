---
description: Проверяет существование всех временных подписчиков в хранилище данных. Вызывая этот метод, можно убедиться, что все временные подписчики, перечисленные в хранилище данных, активны.
ms.assetid: fffdde33-e960-42ef-a089-8ea8a6f33d52
title: 'Метод IEventSystem2:: Верифитрансиентсубскриберс'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IEventSystem2.VerifyTransientSubscribers
api_type:
- COM
api_location: ''
ms.openlocfilehash: 9b147a8910ef3574b93389088af798a84265dd7f929b458e9bd94232cc586a17
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120070614"
---
# <a name="ieventsystem2verifytransientsubscribers-method"></a>Метод IEventSystem2:: Верифитрансиентсубскриберс

Проверяет существование всех временных подписчиков в хранилище данных. Вызывая этот метод, можно убедиться, что все временные подписчики, перечисленные в хранилище данных, активны.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT VerifyTransientSubscribers();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод может возвращать стандартные возвращаемые значения E \_ INVALIDARG, e \_ OUTOFMEMORY, e \_ непредвиденные, e \_ Fail и S \_ ОК.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/> |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>       |



## <a name="see-also"></a>См. также

<dl> <dt>

[**IEventSystem2**](ieventsystem2.md)
</dt> </dl>

 

 




