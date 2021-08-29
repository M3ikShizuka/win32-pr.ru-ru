---
description: Метод Get \_ сркоффсеткс извлекает горизонтальное смещение исходного прямоугольника.
ms.assetid: 528a5306-86bd-4ae2-ad03-57247362c5b5
title: 'Метод Идксткомпоситор:: get_SrcOffsetX (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IDxtCompositor.get_SrcOffsetX
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: b66748c9c7114659d410558b2931bc64e9f3bd41b1e62b7fa265ae166a91d6ba
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119427984"
---
# <a name="idxtcompositorget_srcoffsetx-method"></a>Метод Идксткомпоситор:: Get \_ сркоффсеткс

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`get_SrcOffsetX`Метод получает горизонтальное смещение исходного прямоугольника.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_SrcOffsetX(
  [out, retval] long *pVal
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Pval* \[ out, retval\]
</dt> <dd>

Получает горизонтальное смещение исходного прямоугольника в пикселях.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

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

 

 




