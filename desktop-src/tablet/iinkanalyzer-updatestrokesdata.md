---
description: Обновляет данные пакета для указанных штрихов.
ms.assetid: 7fca4c39-eef2-4019-86a0-27cd0e4e7510
title: 'Метод Иинканализер:: Упдатестрокесдата (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IInkAnalyzer.UpdateStrokesData
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: 497a026dc82031834588ffcd81e9aee2a6e9f0c8ff1c2971567c934ae66105af
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119713324"
---
# <a name="iinkanalyzerupdatestrokesdata-method"></a>Метод Иинканализер:: Упдатестрокесдата

Обновляет данные пакета для указанных штрихов.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT UpdateStrokesData(
  [in] ULONG ulStrokeIdsCount,
  [in] LONG  *plStrokeIds,
  [in] ULONG ulStrokePacketDescriptionCount,
  [in] GUID  *pStrokePacketDescriptionGuids,
  [in] ULONG *pulPacketDataCountPerStroke,
  [in] LONG  *plStrokePacketData
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*улстрокеидскаунт* \[ окне\]
</dt> <dd>

Число штрихов для обновления.

</dd> <dt>

*плстрокеидс* \[ окне\]
</dt> <dd>

Массив, содержащий идентификаторы штрихов.

</dd> <dt>

*улстрокепаккетдескриптионкаунт* \[ окне\]
</dt> <dd>

Число свойств в каждом пакете.

</dd> <dt>

*пстрокепаккетдескриптионгуидс* \[ окне\]
</dt> <dd>

Массив, содержащий идентификаторы свойств пакета.

</dd> <dt>

*пулпаккетдатакаунтперстроке* \[ окне\]
</dt> <dd>

Массив, содержащий количество пакетов в каждом штрихе.

</dd> <dt>

*плстрокепаккетдата* \[ окне\]
</dt> <dd>

Массив, содержащий данные пакета для штрихов.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Remarks

параметр *плстрокепаккетдата* содержит данные пакетов для всех штрихов. Параметр *пстрокепаккетдескриптионгуидс* содержит глобальные уникальные идентификаторы (GUID), которые описывают типы данных пакетов, включаемые для каждой точки в каждом штрихе. Полный список доступных свойств пакетов см. в разделе [константы паккетпропертигуидс](packetpropertyguids-constants.md).

Только штрихи с одинаковыми описаниями пакетов могут быть обновлены в одном вызове **метода иинканализер:: упдатестрокесдата**.

Этот метод не обновляет «грязную» область анализатора рукописного ввода (см. раздел [**метод иинканализер:: жетдиртирегион**](iinkanalyzer-getdirtyregion.md)).

Если указанный штрих не связан с [**иинканализер**](iinkanalyzer.md), этот метод игнорирует идентификатор.

Если ни один из указанных штрихов не определяет штрих, связанный с [**иинканализер**](iinkanalyzer.md), этот метод возвращает значение без обновления **иинканализер**.

Этот метод возвращает код ошибки, если *плстрокеидс* имеет **значение NULL**.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                     |
| Заголовок<br/>                   | <dl> <dt>Иаком. h (также требуется Иаком \_ i. c)</dt> </dl> |
| DLL<br/>                      | <dl> <dt>IACom.dll</dt> </dl>                          |



## <a name="see-also"></a>См. также

<dl> <dt>

[**иинканализер**](iinkanalyzer.md)
</dt> <dt>

[**Метод Иинканализер:: Аддстроке**](iinkanalyzer-addstroke.md)
</dt> <dt>

[**Метод Иинканализер:: Аддстрокефорлангуаже**](iinkanalyzer-addstrokeforlanguage.md)
</dt> <dt>

[**Метод Иинканализер:: Аддстрокетокустомрекогнизер**](iinkanalyzer-addstroketocustomrecognizer.md)
</dt> <dt>

[**Метод Иинканализер:: Аддстрокес**](iinkanalyzer-addstrokes.md)
</dt> <dt>

[**Метод Иинканализер:: Аддстрокесфорлангуаже**](iinkanalyzer-addstrokesforlanguage.md)
</dt> <dt>

[**Метод Иинканализер:: Аддстрокестокустомрекогнизер**](iinkanalyzer-addstrokestocustomrecognizer.md)
</dt> <dt>

[**Метод Иинканализер:: Клеарстрокедата**](iinkanalyzer-clearstrokedata.md)
</dt> <dt>

[**\_Ианалисисевентс:: Упдатестрокескаче**](-ianalysisevents-updatestrokescache.md)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

 




