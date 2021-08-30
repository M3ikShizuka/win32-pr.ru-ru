---
description: Функция обратного вызова, используемая для уведомления узла о завершении автономного анализа.
MS-HAID: vspixengine.IOfflineAnalysisCallback\_OfflineAnalysisComplete\_DWORD\_HRESULT\_BSTR
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: 'Метод Иоффлинеаналисискаллбакк:: Оффлинеаналисискомплете'
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: 36E10709-51DC-4657-B184-F1F807ABBBB4
api_name:
- IOfflineAnalysisCallback.OfflineAnalysisComplete
api_type:
- COM
api_location:
- vspixengine.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: 8829fbb94800a295f5e13ad2ec3c907c64fbfc93
ms.sourcegitcommit: c276a8912787b2cda74dcf54eb96df961bb1188b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2021
ms.locfileid: "122624150"
---
# <a name="span-idvspixengineiofflineanalysiscallback_offlineanalysiscomplete_dword_hresult_bstrspaniofflineanalysiscallbackofflineanalysiscomplete-method"></a><span id="vspixengine.iofflineanalysiscallback_offlineanalysiscomplete_dword_hresult_bstr"></span>Метод Иоффлинеаналисискаллбакк:: Оффлинеаналисискомплете

Функция обратного вызова, используемая для уведомления узла о завершении автономного анализа.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT OfflineAnalysisComplete(
   DWORD   cookie,
   HRESULT result,
   BSTR    outputFullFileName
);
```

## <a name="parameters"></a>Параметры

*"*   
Файл cookie, который однозначно определяет запрос, который инициировал анализ в автономном режиме.

*результат*   
Указывает, завершился ли автономный анализ успешно или нет. В случае успеха результаты были записаны в файл.

*аутпутфуллфиленаме*   
Строка COM, контианинг имя файла, в котором были записаны результаты автономного анализа.

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования

<table><colgroup><col  /><col  /></colgroup><tbody><tr class="odd"><td><p>Заголовок</p></td><td>Вспиксенгине. h</td></tr></tbody></table>

## <a name="span-idsee_alsospansee-also"></a><span id="see_also"></span> См. также

[**иоффлинеаналисискаллбакк**](/windows/desktop/direct3dtools/iofflineanalysiscallback)

 

 
