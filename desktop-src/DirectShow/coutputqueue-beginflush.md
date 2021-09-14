---
description: Каутпуткуеуе. Бегинфлуш, метод Бегинфлуш начинает операцию очистки.
ms.assetid: d37b611e-742f-4bdf-bd72-a91cd1c473b3
title: Каутпуткуеуе. Бегинфлуш, метод (Аутпутк. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- COutputQueue.BeginFlush
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: e7c6168daf766ec11e18e86673d9d25542b50462
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127346986"
---
# <a name="coutputqueuebeginflush-method"></a>Каутпуткуеуе. Бегинфлуш, метод

`BeginFlush`Метод начинает операцию записи на диск.

## <a name="syntax"></a>Синтаксис


```C++
void BeginFlush();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод задает для переменной члена [**каутпуткуеуе:: m \_ Бфлушинг**](coutputqueue-m-bflushing.md) **значение true**. Если объект использует поток, поток вызывает метод [**каутпуткуеуе:: фрисамплес**](coutputqueue-freesamples.md) , чтобы освободить все ожидающие выборки. В противном случае объект вызывает **фрисамплес** во время метода [**Каутпуткуеуе:: ендфлуш**](coutputqueue-endflush.md) . Этот метод также задает значение false для переменной члена [**каутпуткуеуе:: m \_ HR**](coutputqueue-m-hr.md) \_ , что приводит к отмене всех новых выборок объектом.

Объект передает уведомление о сбросе на диск, вызывая метод [**Ипин:: бегинфлуш**](/windows/desktop/api/Strmif/nf-strmif-ipin-beginflush) для входного ПИН-кода.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>аутпутк. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Каутпуткуеуе**](coutputqueue.md)
</dt> </dl>

 

 




