---
description: Метод размещения \_ сркоффсеткс задает горизонтальное смещение исходного прямоугольника.
ms.assetid: 54f38dfd-3804-4ce4-ac70-5c7933e1a03f
title: 'Идксткомпоситор: метод ut_SrcOffsetX:p (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IDxtCompositor.put_SrcOffsetX
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: a23cf2a07a209509cf55129ecd77ee8e035f5341
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126891832"
---
# <a name="idxtcompositorput_srcoffsetx-method"></a>Идксткомпоситор::p UT \_ сркоффсеткс метод

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`put_SrcOffsetX`Метод задает горизонтальное смещение исходного прямоугольника.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_SrcOffsetX(
  [in] long newVal
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*неввал* \[ окне\]
</dt> <dd>

Горизонтальное смещение исходного прямоугольника в пикселях.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Комментарии

> [!Note]  
> Файл заголовка Кедит. h несовместим с заголовками Direct3D позднее версии 7.

 

> [!Note]  
> чтобы получить кедит. h, скачайте [обновление Microsoft Windows SDK для Windows Vista и платформа .NET Framework 3,0](https://msdn.microsoft.com/windowsvista/bb980924.aspx). кедит. h недоступен в Microsoft Windows SDK для Windows 7 и платформа .NET Framework 3,5 с пакетом обновления 1 (sp1).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Кедит. h</dt> </dl>      |
| Библиотека<br/> | <dl> <dt>Стрмиидс. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Идксткомпоситор**](idxtcompositor.md)
</dt> </dl>

 

 




