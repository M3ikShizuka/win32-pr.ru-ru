---
description: Происходит после того, как Иинканализер обновляет одно или несколько свойств объекта Иконтекстноде.
ms.assetid: f626c263-31a4-45ee-ae04-3251eac0d652
title: 'Событие _IAnalysisProxyEvents:: Контекстнодепропертиесупдатед (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- _IAnalysisProxyEvents.ContextNodePropertiesUpdated
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: e2ed15da1c2eaf38ed8ac0617756ddb85d713f490b1a3a26af0db11da834b206
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119337214"
---
# <a name="_ianalysisproxyeventscontextnodepropertiesupdated-event"></a>\_Событие Ианалисиспроксевентс:: Контекстнодепропертиесупдатед

Происходит после того, как [**иинканализер**](iinkanalyzer.md) обновляет одно или несколько свойств объекта [**иконтекстноде**](icontextnode.md) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT ContextNodePropertiesUpdated(
  [in] IInkAnalyzer *pInkAnalyzer,
  [in] IContextNode *pContextNodeUpdated
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пинканализер* \[ окне\]
</dt> <dd>

Объект [**иинканализер**](iinkanalyzer.md) , обновляющий свойства.

</dd> <dt>

*пконтекстнодеупдатед* \[ окне\]
</dt> <dd>

Объект [**иконтекстноде**](icontextnode.md) , свойства которого обновляются.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Remarks

Это событие используется, когда приложение поддерживает собственную структуру данных, которая синхронизируется с [**иинканализер**](iinkanalyzer.md). Это событие возникает на этапе выверки анализа рукописного текста или в ответ на метод анализатора рукописного ввода, который изменяет свойства [**иконтекстноде**](icontextnode.md) (см. [**Иконтекстноде:: жетпропертидата**](icontextnode-getpropertydata.md)).

Дополнительные сведения о синхронизации данных приложения с помощью [**иинканализер**](iinkanalyzer.md)см. в разделе [учетная запись-посредник данных с помощью анализа рукописного ввода](data-proxy-with-ink-analysis.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                     |
| Header<br/>                   | <dl> <dt>Иаком. h (также требуется Иаком \_ i. c)</dt> </dl> |
| DLL<br/>                      | <dl> <dt>IACom.dll</dt> </dl>                          |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_ианалисиспроксевентс**](-ianalysisproxyevents.md)
</dt> <dt>

[**иинканализер**](iinkanalyzer.md)
</dt> <dt>

[**иконтекстноде**](icontextnode.md)
</dt> <dt>

[**Метод Иинканализер:: Analyze**](iinkanalyzer-analyze.md)
</dt> <dt>

[**Метод Иинканализер:: Баккграунданализе**](iinkanalyzer-backgroundanalyze.md)
</dt> <dt>

[Свойства узла контекста](context-node-properties.md)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

 




