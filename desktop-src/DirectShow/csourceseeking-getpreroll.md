---
description: 'Метод Жетпреролл извлекает время предвыполнения. Этот метод реализует метод Имедиасикинг:: Жетпреролл.'
ms.assetid: 2395d5b2-8c1f-40cd-8d4a-48620debe7a7
title: Ксаурцесикинг. Жетпреролл, метод (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSourceSeeking.GetPreroll
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 097af089a7221f005cf7f3aac74953166af3cb2a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053951"
---
# <a name="csourceseekinggetpreroll-method"></a>Ксаурцесикинг. Жетпреролл, метод

`GetPreroll`Метод получает время предизвлечения. Этот метод реализует метод [**имедиасикинг:: жетпреролл**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-getpreroll) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetPreroll(
   LONGLONG *pPreroll
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппреролл* 
</dt> <dd>

Указатель на переменную, которая получает время предвыполнения. Значение равно нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из значений **HRESULT** , перечисленных в следующей таблице.



| Код возврата                                                                               | Описание                       |
|-------------------------------------------------------------------------------------------|-----------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>      | Успешное завершение<br/>                |
| <dl> <dt>**\_указатель E**</dt> </dl> | Значение указателя **null**<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ксаурцесикинг**](csourceseeking.md)
</dt> </dl>

 

 




