---
description: Извлекает все подсказку анализа, Иконтекстноде объекты, присоединенные к Иинканализер, с указанным именем.
ms.assetid: 15269ee0-055c-424e-be49-945f47e8a77e
title: 'Метод Иинканализер:: Жетаналисишинтсбинаме (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IInkAnalyzer.GetAnalysisHintsByName
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: d86b18bfb8cf17097a36e35fc638dd9bd763d243
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127344854"
---
# <a name="iinkanalyzergetanalysishintsbyname-method"></a>Метод Иинканализер:: Жетаналисишинтсбинаме

Извлекает все подсказку анализа, [**иконтекстноде**](icontextnode.md) объекты, присоединенные к [**иинканализер**](iinkanalyzer.md) , с указанным именем.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetAnalysisHintsByName(
  [in]  BSTR          hintName,
  [out] IContextNodes **ppAnalysisHints
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*хинтнаме* \[ окне\]
</dt> <dd>

Имя подсказки для поиска.

</dd> <dt>

*ппаналисишинтс* \[ заполняет\]
</dt> <dd>

Подсказка анализа [**иконтекстноде**](icontextnode.md) объекты в [**иинканализер**](iinkanalyzer.md) с указанным именем.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописных данных](classes-and-interfaces---ink-analysis.md) возвращаемые значения.

## <a name="remarks"></a>Комментарии

> [!Caution]  
> Чтобы избежать утечки памяти, вызовите метод [**IUnknown:: Release**](/windows/desktop/api/unknwn/nf-unknwn-iunknown-release) в *ппаналисишинтс* , когда больше не нужно использовать объект.

 

Этот метод возвращает пустую коллекцию, если такие узлы подсказок по анализу не присоединены к [**иинканализер**](iinkanalyzer.md).

Узел указания анализа — это [**иконтекстноде**](icontextnode.md) с типом узла контекста аналисишинт (см. раздел [**Иконтекстноде:: GetType**](icontextnode-gettype.md) и [типы узлов контекста](context-node-types.md)).

Чтобы добавить сведения о контексте в указание, используйте [**иконтекстноде:: аддпропертидата**](icontextnode-addpropertydata.md) с параметром *ппропертидатаид* , равным одному из глобальных уникальных идентификаторов (GUID) в константах [свойств указания анализа](analysis-hint-properties.md) .

Чтобы определить, какие значения свойств установлены в узле контекста, используйте [**иконтекстноде:: жетпропертидатаидс**](icontextnode-getpropertydataids.md). Чтобы найти значение свойства, используйте [**иконтекстноде:: жетпропертидата**](icontextnode-getpropertydata.md).

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

[**иконтекстноде**](icontextnode.md)
</dt> <dt>

[**Метод Иинканализер:: Креатеаналисишинт**](iinkanalyzer-createanalysishint.md)
</dt> <dt>

[**Иинканализер: метод:D Елетеаналисишинт**](iinkanalyzer-deleteanalysishint.md)
</dt> <dt>

[**Метод Иинканализер:: Жетаналисишинтс**](iinkanalyzer-getanalysishints.md)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

