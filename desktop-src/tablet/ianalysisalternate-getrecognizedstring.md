---
description: Возвращает распознанное строковое значение объекта Ианалисисалтернате.
ms.assetid: cdf41824-77a4-4c71-8712-f380a6cbf4c5
title: 'Метод Ианалисисалтернате:: Жетрекогнизедстринг (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAnalysisAlternate.GetRecognizedString
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: 5489773b29ade35d4b7297065c1104bfecefa117
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127256783"
---
# <a name="ianalysisalternategetrecognizedstring-method"></a>Метод Ианалисисалтернате:: Жетрекогнизедстринг

Возвращает распознанное строковое значение объекта [**ианалисисалтернате**](ianalysisalternate.md) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetRecognizedString(
  [out] BSTR *pbstrRecognizedString
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пбстррекогнизедстринг* \[ заполняет\]
</dt> <dd>

Указатель на строку **BSTR** , для которой задано распознанное строковое значение.

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

[**ианалисисалтернате**](ianalysisalternate.md)
</dt> <dt>

[**Метод Иинканализер:: Жетрекогнизедстринг**](iinkanalyzer-getrecognizedstring.md)
</dt> </dl>

 

 




