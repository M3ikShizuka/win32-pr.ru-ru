---
description: Метод Препарепалетте настраивает палитру на основе типа носителя из фильтра-владельца.
ms.assetid: cb012391-39ab-4ad1-aeb7-ec25010ac64a
title: Цимажепалетте. Препарепалетте, метод (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CImagePalette.PreparePalette
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: a9b09804b2ee6ad9fbda394a7fb8f9f188b46453
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127273104"
---
# <a name="cimagepalettepreparepalette-method"></a>Цимажепалетте. Препарепалетте, метод

`PreparePalette`Метод настраивает палитру на основе типа носителя из фильтра-владельца.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT PreparePalette(
   const CMediaType *pmtNew,
   const CMediaType *pmtOld,
         LPSTR      szDevice
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пмтнев* 
</dt> <dd>

Указатель на новый тип носителя. Блок формата должен быть структурой [**видеоинфохеадер**](/previous-versions/windows/desktop/api/amvideo/ns-amvideo-videoinfoheader) .

</dd> <dt>

*пмтолд* 
</dt> <dd>

Указатель на старый тип носителя. Если тип носителя задается в первый раз, этот параметр может быть пустым типом без блока Format. В противном случае блок формата должен быть структурой **видеоинфохеадер** .

</dd> <dt>

*сздевице* 
</dt> <dd>

Указатель на строку, содержащую имя устройства вывода, которое возвращается функцией GDI **енумдисплайдевицес** . Чтобы использовать основное устройство вывода, присвойте этому параметру **значение NULL**.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ ОК, если палитра была обновлена, или \_ значение false, если палитра не изменилась.

## <a name="remarks"></a>Комментарии

Если необходимо обновить палитру, этот метод выполняет следующие действия:

-   Вызывает [**Цимажепалетте:: макепалетте**](cimagepalette-makepalette.md) для создания новой логической палитры.
-   отправляет событие [**\_ \_ изменения палитры EC**](ec-palette-changed.md) в фильтр Graph Manager.
-   Вызывает [**кбасевиндов:: сетпалетте**](cbasewindow-setpalette.md) для объекта **кбасевиндов** .
-   Вызывает [**кдравимаже:: инкрементпалеттеверсион**](cdrawimage-incrementpaletteversion.md) для объекта **кдравимаже** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Цимажепалетте**](cimagepalette.md)
</dt> </dl>

 

 




