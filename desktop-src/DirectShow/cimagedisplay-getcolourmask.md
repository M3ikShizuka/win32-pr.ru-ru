---
description: Метод Жетколаурмаск извлекает цветовую маску для текущего формата экрана.
ms.assetid: 386d0439-8502-411d-935c-3c2153a8b5b4
title: Цимажедисплай. Жетколаурмаск, метод (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CImageDisplay.GetColourMask
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 499b3677cd68444b58514d692d87cd4f631350b6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170027"
---
# <a name="cimagedisplaygetcolourmask-method"></a>Цимажедисплай. Жетколаурмаск, метод

`GetColourMask`Метод извлекает цветовую маску для текущего формата экрана.

## <a name="syntax"></a>Синтаксис


```C++
BOOL GetColourMask(
   DWORD *pMaskRed,
   DWORD *pMaskGreen,
   DWORD *pMaskBlue
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пмаскред* 
</dt> <dd>

Указатель на переменную, получающую маску красного компонента.

</dd> <dt>

*пмаскгрин* 
</dt> <dd>

Указатель на переменную, которая получает маску зеленого компонента.

</dd> <dt>

*пмаскблуе* 
</dt> <dd>

Указатель на переменную, получающую маску синего компонента.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Цимажедисплай**](cimagedisplay.md)
</dt> </dl>

 

 




