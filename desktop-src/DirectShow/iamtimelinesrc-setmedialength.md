---
description: Метод Сетмедиаленгс задает длительность исходного файла.
ms.assetid: 0a68ad50-91d5-4cb3-95ef-35b9460ac3e4
title: 'Метод Иамтимелинесрк:: Сетмедиаленгс (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineSrc.SetMediaLength
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: d2e4b608fea02ac8a7424e980ba3d3e63105e88bc0689d0ea281415bd14d00e4
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120051664"
---
# <a name="iamtimelinesrcsetmedialength-method"></a>Метод Иамтимелинесрк:: Сетмедиаленгс

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`SetMediaLength`Метод задает длительность исходного файла.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetMediaLength(
   REFERENCE_TIME Length
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Длина* 
</dt> <dd>

Длина носителя (в 100-наносекундных единицах).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

Можно избежать потенциальных ошибок отрисовки, установив длину носителя до того, как будет задано время окончания носителя. При задании времени окончания передачи данных DES проверяет его на соответствие длине носителя.

Этот метод не проверяет параметр *длины* , но значение должно равняться фактической длительности исходного файла. Получите длительность исходного файла, вызвав [**имедиадет:: Get \_ стреамленгс**](imediadet-get-streamlength.md).

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

[**Интерфейс Иамтимелинесрк**](iamtimelinesrc.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




