---
description: Изменяет флаги, определяющие, как Иинканализер выполняет анализ рукописного ввода.
ms.assetid: cb82edd0-1f15-4313-a286-1fcd715ac6df
title: 'Метод Иинканализер:: Сетаналисисмодес (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IInkAnalyzer.SetAnalysisModes
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: 826d31fd5b61db2332ef953d55b2cf6c6331995b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570403"
---
# <a name="iinkanalyzersetanalysismodes-method"></a>Метод Иинканализер:: Сетаналисисмодес

Изменяет флаги, определяющие, как [**иинканализер**](iinkanalyzer.md) выполняет анализ рукописного ввода.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetAnalysisModes(
  [in] AnalysisModes analysisMode
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*аналисисмоде* \[ окне\]
</dt> <dd>

Побитовое сочетание значений перечисления [**аналисисмодес**](analysismodes.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                     |
| Заголовок<br/>                   | <dl> <dt>Иаком. h (также требуется Иаком \_ i. c)</dt> </dl> |
| DLL<br/>                      | <dl> <dt>IACom.dll</dt> </dl>                          |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**иинканализер**](iinkanalyzer.md)
</dt> <dt>

[**аналисисмодес**](analysismodes.md)
</dt> <dt>

[**Метод Иинканализер:: Analyze**](iinkanalyzer-analyze.md)
</dt> <dt>

[**Метод Иинканализер:: Баккграунданализе**](iinkanalyzer-backgroundanalyze.md)
</dt> <dt>

[**Метод Иинканализер:: Жетаналисисмодес**](iinkanalyzer-getanalysismodes.md)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

 




