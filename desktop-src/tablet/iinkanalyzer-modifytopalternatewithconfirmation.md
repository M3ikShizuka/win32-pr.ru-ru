---
description: Изменяет текущий верхний альтернативный вариант на указанный Ианалисисалтернате.
ms.assetid: 0867a662-d172-4ca2-a41f-49c0ea454768
title: 'Метод Иинканализер:: Модифитопалтернатевисконфирматион (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IInkAnalyzer.ModifyTopAlternateWithConfirmation
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: d7c0b98c0abafeb82e56124dc105ac5204dc4322586db200cb54827173ca6c54
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119773554"
---
# <a name="iinkanalyzermodifytopalternatewithconfirmation-method"></a>Метод Иинканализер:: Модифитопалтернатевисконфирматион

Изменяет текущий верхний альтернативный вариант на указанный [**ианалисисалтернате**](ianalysisalternate.md).

## <a name="syntax"></a>Синтаксис


```C++
HRESULT ModifyTopAlternateWithConfirmation(
  [in] IAnalysisAlternate *alternate,
  [in] VARIANT_BOOL       fconfirmAutomatically
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*альтернативный вариант* \[ окне\]
</dt> <dd>

Альтернативный анализ, который можно задать в качестве нового верхнего альтернативного.

</dd> <dt>

*фконфирмаутоматикалли* \[ окне\]
</dt> <dd>

**Вариант \_ Значение TRUE** , чтобы задать все узлы конечного контекста, которые соответствуют анализу, альтернативному типу подтверждения **конфирматионтипе \_ нодетипеандпропертиес** (см [**. Иконтекстноде:: Confirm**](icontextnode-isconfirmed.md) и [**конфирматионтипе**](confirmationtype.md)); **Вариант \_ Значение FALSE** , чтобы задать все узлы конечного контекста, которые соответствуют анализу, альтернативному типу подтверждения **конфирматионтипе \_ None**.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Remarks

Для получения вариантов анализа используйте метод [**иинканализер:: alternate**](iinkanalyzer-getalternates.md), [**Иинканализер:: Жеталтернатесфорконтекстнодес**](iinkanalyzer-getalternatesforcontextnodes.md)или [**метод иинканализер:: жеталтернатесфорстрокес**](iinkanalyzer-getalternatesforstrokes.md). Чтобы получить объекты узла контекста, связанные с альтернативным анализом, используйте [**метод ианалисисалтернате:: жеталтернатенодес**](ianalysisalternate-getalternatenodes.md).

Чтобы изменить тип подтверждения для контекстного узла, используйте [**иконтекстноде:: Confirm**](icontextnode-confirm.md).

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

[**ианалисисалтернате**](ianalysisalternate.md)
</dt> <dt>

[**иконтекстноде**](icontextnode.md)
</dt> <dt>

[**Анализ рукописного ввода Конфирматионтипе**](confirmationtype.md)
</dt> <dt>

[Ссылки](ink-analysis-reference.md)
</dt> </dl>

 

 




