---
description: Создает копию Ианалисисрегион.
ms.assetid: eb94e1ce-7801-409d-9ae6-e7db0a9b861f
title: 'Метод Ианалисисрегион:: Clone (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAnalysisRegion.Clone
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: fb069ddb461ab4422f8cbbc8990fb6d735808e62
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460243"
---
# <a name="ianalysisregionclone-method"></a>Метод Ианалисисрегион:: Clone

Создает копию [**ианалисисрегион**](ianalysisregion.md).

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Clone(
  [out] IAnalysisRegion **pClonedRegion
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пклонедрегион* \[ заполняет\]
</dt> <dd>

Указатель на копию [**ианалисисрегион**](ianalysisregion.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Remarks

Этот метод екивалентся в Сесистем. Windows. метод Ink. аналисискоре. аналисисрегионбасе. Clone в платформа .NET Framework.

> [!Caution]  
> Чтобы избежать утечки памяти, вызовите метод [**IUnknown:: Release**](/windows/desktop/api/unknwn/nf-unknwn-iunknown-release) в \* *пклонедрегион* , когда больше не нужно использовать клонированный регион анализа.

 

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

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

