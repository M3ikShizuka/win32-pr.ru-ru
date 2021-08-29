---
description: 'Ксаурцесикинг. Сеттимеформат, метод Сеттимеформат задает формат времени. Этот метод реализует метод Имедиасикинг:: Сеттимеформат.'
ms.assetid: dbc7c950-8cc2-4f8e-adfa-8f5cdc1b56c7
title: Ксаурцесикинг. Сеттимеформат, метод (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSourceSeeking.SetTimeFormat
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: b4fc3e4fef02b5ed2a0d531c48d9503d4703d16e4353f46ff5b233bc12ebab16
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119526124"
---
# <a name="csourceseekingsettimeformat-method"></a>Ксаурцесикинг. Сеттимеформат, метод

`SetTimeFormat`Метод задает формат времени. Этот метод реализует метод [**имедиасикинг:: сеттимеформат**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-settimeformat) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetTimeFormat(
   const GUID *pFormat
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пформат* 
</dt> <dd>

Указатель на GUID формата времени. См. раздел [**идентификаторы GUID формата времени**](time-format-guids.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из значений **HRESULT** , перечисленных в следующей таблице.



| Код возврата                                                                                  | Описание                                   |
|----------------------------------------------------------------------------------------------|-----------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>         | Успешно.<br/>                           |
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl> | Указанный формат не поддерживается.<br/> |
| <dl> <dt>**\_указатель E**</dt> </dl>    | **Пустой** аргумент указателя.<br/>         |



 

## <a name="remarks"></a>Remarks

Единственный формат времени, поддерживаемый базовым классом, — это \_ \_ время носителя формата времени \_ (100-наносекундных единиц).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Ксаурцесикинг**](csourceseeking.md)
</dt> </dl>

 

 




