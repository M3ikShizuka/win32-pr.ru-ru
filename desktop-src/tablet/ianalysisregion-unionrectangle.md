---
description: Разворачивает область этого Ианалисисрегиона в область, созданную его объединением с указанным прямоугольником.
ms.assetid: 9b12f509-4f6a-43b0-9639-bef060fd6d50
title: 'Метод Ианалисисрегион:: Унионректангле (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAnalysisRegion.UnionRectangle
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: 3a28a60eae95641225dd9c01791d89a9c38ada82
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460242"
---
# <a name="ianalysisregionunionrectangle-method"></a>Метод Ианалисисрегион:: Унионректангле

Разворачивает область этого [**ианалисисрегиона**](ianalysisregion.md) в область, созданную его объединением с указанным прямоугольником.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT UnionRectangle(
  [in] RECT *pRectangle
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пректангле* \[ окне\]
</dt> <dd>

Указатель на прямоугольник, с которым выполняется объединение, в координатах рукописного ввода.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Remarks

Координаты прямоугольника находятся в единицах HIMETRIC.

Если любая из этих областей бесконечно, Новая область также будет бесконечна.

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

[**Ианалисисрегион:: Ексклудеректангле**](ianalysisregion-excluderectangle.md)
</dt> <dt>

[**Метод Ианалисисрегион:: Ексклудерегион**](ianalysisregion-excluderegion.md)
</dt> <dt>

[**Метод Ианалисисрегион:: Интерсектректангле**](ianalysisregion-intersectrectangle.md)
</dt> <dt>

[**Метод Ианалисисрегион:: Интерсектрегион**](ianalysisregion-intersectregion.md)
</dt> <dt>

[**Метод Ианалисисрегион:: Унионрегион**](ianalysisregion-unionregion.md)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

 




