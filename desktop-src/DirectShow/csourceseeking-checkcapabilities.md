---
description: 'Метод Чекккапабилитиес запрашивает, есть ли у потока указанные возможности поиска. Этот метод реализует метод Имедиасикинг:: Чекккапабилитиес.'
ms.assetid: 5d37e179-9e04-44e1-acbc-dfd2682830c0
title: Ксаурцесикинг. Чекккапабилитиес, метод (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSourceSeeking.CheckCapabilities
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 332e5fc461a39eff7ebfc70aa32a9a4d1a28a6928c15f6222e3804e2a542f6ed
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120087054"
---
# <a name="csourceseekingcheckcapabilities-method"></a>Ксаурцесикинг. Чекккапабилитиес, метод

`CheckCapabilities`Метод запрашивает, имеет ли поток указанные возможности поиска. Этот метод реализует метод [**имедиасикинг:: чекккапабилитиес**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-checkcapabilities) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT CheckCapabilities(
   DWORD *pCapabilities
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пкапабилитиес* 
</dt> <dd>

Указатель на побитовую комбинацию одного или нескольких атрибутов [**\_ \_ \_ возможностей**](/windows/win32/api/strmif/ne-strmif-am_seeking_seeking_capabilities) поиска.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из значений **HRESULT** , перечисленных в следующей таблице.



| Код возврата                                                                               | Описание                                                            |
|-------------------------------------------------------------------------------------------|------------------------------------------------------------------------|
| <dl> <dt>**S \_ false**</dt> </dl>   | Существуют не все возможности в *пкапабилитиес* .<br/> |
| <dl> <dt>**\_ОК**</dt> </dl>      | В *пкапабилитиес* есть все возможности.<br/>            |
| <dl> <dt>**\_указатель E**</dt> </dl> | **Пустой** аргумент указателя.<br/>                                  |



 

## <a name="remarks"></a>Remarks

Как реализованный, этот метод проверяет значение *\* пкапабилитиес* на соответствие переменной члена [**ксаурцесикинг:: m \_ двсикингкапс**](csourceseeking-m-dwseekingcaps.md) . Однако он не устанавливает *\* пкапабилитиес* равным **m \_ двсикингкапс**, как описано в методе [**имедиасикинг:: чекккапабилитиес**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-checkcapabilities) . Кроме того, в случае, если ни одна из указанных возможностей не доступна, метод не возвращает значение E \_ Failed. Более полная реализация будет выглядеть следующим образом:


```C++
STDMETHODIMP CheckCapabilities(DWORD *pCapabilities)
{
    CheckPointer(pCapabilities, E_POINTER)
;
    DWORD dwCaps;
    HRESULT hr = GetCapabilities(&dwCaps);
    if (SUCCEEDED(hr))
    {
        dwCaps &= *pCapabilities;
        if (dwCaps)
        {
            hr =  (dwCaps == *pCapabilities ? S_OK : S_FALSE );
        }
        else 
        {
            hr = E_FAIL;
        }
        *pCapabilities = dwCaps;
    }
    else 
    {
        *pCapabilities = 0;
    }
    return hr;
}
```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Ксаурцесикинг**](csourceseeking.md)
</dt> </dl>

 

 




