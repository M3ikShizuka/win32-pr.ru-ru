---
description: Извлекает объект Ианалисисалтернате по указанному индексу в коллекции.
ms.assetid: d927e2f1-ca21-415d-90ad-d1ded575fcb7
title: 'Метод Ианалисисалтернатес:: Жетаналисисалтернате (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAnalysisAlternates.GetAnalysisAlternate
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: ab0ccc52bcb390e27f78dd14ec19857c2065b92f7b1b0eb67a34fedf952f4e94
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119940653"
---
# <a name="ianalysisalternatesgetanalysisalternate-method"></a>Метод Ианалисисалтернатес:: Жетаналисисалтернате

Извлекает объект [**ианалисисалтернате**](ianalysisalternate.md) по указанному индексу в коллекции.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetAnalysisAlternate(
  [in]  ULONG              ulIndex,
  [out] IAnalysisAlternate **ppAlternate
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*улиндекс* \[ окне\]
</dt> <dd>

Отсчитываемый от нуля индекс объекта [**ианалисисалтернате**](ianalysisalternate.md) , который необходимо получить.

</dd> <dt>

*ппалтернате* \[ заполняет\]
</dt> <dd>

Указатель на объект [**ианалисисалтернате**](ianalysisalternate.md) по указанному индексу в коллекции.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Remarks

> [!Caution]  
> Чтобы избежать утечки памяти, вызовите метод [**IUnknown:: Release**](/windows/desktop/api/unknwn/nf-unknwn-iunknown-release) в \* *ппалтернате* , когда больше не нужно использовать альтернативный анализ.

 

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                     |
| Заголовок<br/>                   | <dl> <dt>Иаком. h (также требуется Иаком \_ i. c)</dt> </dl> |
| DLL<br/>                      | <dl> <dt>IACom.dll</dt> </dl>                          |



## <a name="see-also"></a>См. также

<dl> <dt>

[**ианалисисалтернатес**](ianalysisalternates.md)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

