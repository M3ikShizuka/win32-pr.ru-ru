---
description: Возвращает все Иконтекстноденые в подсказках анализа объекты, присоединенные к Иинканализер.
ms.assetid: 97cff025-3d9e-4137-b1ac-635153804744
title: 'Метод Иинканализер:: Жетаналисишинтс (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IInkAnalyzer.GetAnalysisHints
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: c5ce66eeb6362ed74f1df1a38f220603d3a30117
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572399"
---
# <a name="iinkanalyzergetanalysishints-method"></a>Метод Иинканализер:: Жетаналисишинтс

Возвращает все [**иконтекстноденые**](icontextnode.md) в подсказках анализа объекты, присоединенные к [**иинканализер**](iinkanalyzer.md).

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetAnalysisHints(
  [out] IContextNodes **ppAnalysisHints
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппаналисишинтс* \[ заполняет\]
</dt> <dd>

Указатель на все подсказку анализа, [**иконтекстноде**](icontextnode.md) объекты в [**иинканализер**](iinkanalyzer.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Комментарии

> [!Caution]  
> Чтобы избежать утечки памяти, вызовите метод [**IUnknown:: Release**](/windows/desktop/api/unknwn/nf-unknwn-iunknown-release) в *ппаналисишинтс* , когда больше не нужно использовать объект.

 

Этот метод возвращает пустую коллекцию, если к [**иинканализер**](iinkanalyzer.md)не присоединены узлы подсказок анализа.

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

[**Метод Иинканализер:: Жетаналисишинтсбинаме**](iinkanalyzer-getanalysishintsbyname.md)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

