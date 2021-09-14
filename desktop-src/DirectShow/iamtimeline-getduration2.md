---
description: Метод GetDuration2 извлекает Длительность временной шкалы. Этот метод эквивалентен Иамтимелине::-Duration, но принимает параметр типа Double.
ms.assetid: 49f5eed3-7fab-4f08-b65c-300349b197cb
title: 'Метод Иамтимелине:: GetDuration2 (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimeline.GetDuration2
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: bc840e642f6c08825f6f53869229e9cc27e87b38
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145010"
---
# <a name="iamtimelinegetduration2-method"></a>Метод Иамтимелине:: GetDuration2

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`GetDuration2`Метод получает Длительность временной шкалы. Этот метод эквивалентен [**иамтимелине::-Duration**](iamtimeline-getduration.md), но принимает параметр типа **Double**.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetDuration2(
   double *pDuration
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пдуратион* 
</dt> <dd>

Получает длительность временной шкалы в долях секунды.

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

[**Интерфейс Иамтимелине**](iamtimeline.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




