---
description: Извлекает массив прямоугольников, определяющих площадь Ианалисисрегион.
ms.assetid: 40de4c27-4b3b-4db3-af08-cb53e638db6b
title: 'Метод Ианалисисрегион:: Жетрегионсканс (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAnalysisRegion.GetRegionScans
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: 6cb8db60b5818f5bc2bc38892912e9ec40af1eb9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127267699"
---
# <a name="ianalysisregiongetregionscans-method"></a>Метод Ианалисисрегион:: Жетрегионсканс

Извлекает массив прямоугольников, определяющих площадь [**ианалисисрегион**](ianalysisregion.md).

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetRegionScans(
  [out] ULONG *pulCount,
  [out] RECT  **pRegionScans
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пулкаунт* \[ заполняет\]
</dt> <dd>

Число прямоугольников, возвращаемых в *прегионсканс*.

</dd> <dt>

*прегионсканс* \[ заполняет\]
</dt> <dd>

Указатель на массив прямоугольников, определяющий площадь [**ианалисисрегион**](ianalysisregion.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Remarks

Если *прегионсканс* передается как **null**, метод **жетрегионсканс** возвращает значение **S \_ ОК** , а число прямоугольников возвращается в *пулкаунт*.

> [!Caution]  
> Чтобы избежать утечки памяти, используйте [**CoTaskMemFree**](/windows/desktop/api/combaseapi/nf-combaseapi-cotaskmemfree) , чтобы освободить память от \* *прегионсканс* , если эта информация больше не нужна.

 

Границы прямоугольников находятся в координатах для рукописного ввода.

Объединение возвращенных прямоугольников представляет область [**ианалисисрегион**](ianalysisregion.md).

## <a name="examples"></a>Примеры

В следующем примере показано, как получить прямоугольники, определяющие область [**ианалисисрегион**](ianalysisregion.md), `region` и как получить только число прямоугольников.


```C++
// Get the count and the rectangles.
ULONG count = 0;
RECT* rects = 0;
region->GetRegionScans(&count, &rects);

// Use rects

::CoTaskMemFree(rects);

// GetRegionScans just gets the count and returns S_OK
ULONG number = 0;
region->GetRegionScans(&number, NULL); 
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                     |
| Заголовок<br/>                   | <dl> <dt>Иаком. h (также требуется Иаком \_ i. c)</dt> </dl> |
| DLL<br/>                      | <dl> <dt>IACom.dll</dt> </dl>                          |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ианалисисрегион**](ianalysisregion.md)
</dt> <dt>

[**Метод Ианалисисрегион:: DataBound**](ianalysisregion-getbounds.md)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

