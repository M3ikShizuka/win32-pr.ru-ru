---
description: Перечисление, используемое для указания типа события.
MS-HAID: vspixengine.EVENTTYPE
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: Перечисление EVENTTYPE
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: F7A6F396-5BC0-4963-ABFD-ACB7AAE475F5
api_name:
- EVENTTYPE
api_type:
- HeaderDef
api_location:
- vspixengine.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: daa61cc8358fb0dc59f4b819e27077c68748b995
ms.sourcegitcommit: c276a8912787b2cda74dcf54eb96df961bb1188b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2021
ms.locfileid: "122624440"
---
# <a name="span-idvspixengineeventtypespaneventtype-enumeration"></a><span id="vspixengine.eventtype"></span>Перечисление EVENTTYPE

Перечисление, используемое для указания типа события.

## <a name="syntax"></a>Синтаксис

```cpp
C++ 
enum EVENTTYPE {
  ET_NONE = 0, 
  ET_SESSIONSTART, 
  ET_SESSIONEND, 
  ET_PROCESSSTART, 
  ET_PROCESSEND, 
  ET_FRAMEBEGIN, 
  ET_FRAMEEND, 
  ET_USEREVENTBEGIN, 
  ET_USEREVENTEND, 
  ET_USERMARKER, 
  ET_CALL, 
  ET_OBJECTCREATION, 
  ET_OBJECTPOPULATION, 
  ET_CALLSYNC, 
  ET_DRAW, 
  ET_DISPATCH 
};
```

## <a name="constants"></a>Константы

<span id="ET_NONE"></span><span id="et_none"></span>**ET \_ нет**  
Значение, соответствующее отсутствию события.

<span id="ET_SESSIONSTART"></span><span id="et_sessionstart"></span>**ET \_ SESSIONSTART**  
Значение, соответствующее событию запуска сеанса.

<span id="ET_SESSIONEND"></span><span id="et_sessionend"></span>**ET \_ сессионенд**  
Значение, соответствующее событию конца сеанса.

<span id="ET_PROCESSSTART"></span><span id="et_processstart"></span>**ET \_ процессстарт**  
Значение, соответствующее событию запуска процесса.

<span id="ET_PROCESSEND"></span><span id="et_processend"></span>**ET \_ процессенд**  
Значение, соответствующее событию завершения процесса.

<span id="ET_FRAMEBEGIN"></span><span id="et_framebegin"></span>**ET \_ фрамебегин**  
Значение, соответствующее событию начала кадра.

<span id="ET_FRAMEEND"></span><span id="et_frameend"></span>**ET \_ фраминд**  
Значение, соответствующее событию конца кадра. Не используется.

<span id="ET_USEREVENTBEGIN"></span><span id="et_usereventbegin"></span>**ET \_ усеревентбегин**  
Значение, соответствующее событию начала пользовательского события.

<span id="ET_USEREVENTEND"></span><span id="et_usereventend"></span>**ET \_ усеревентенд**  
Значение, соответствующее событию окончания события пользователя. Не используется.

<span id="ET_USERMARKER"></span><span id="et_usermarker"></span>**ET \_ усермаркер**  
Значение, соответствующее событию маркера пользователя.

<span id="ET_CALL"></span><span id="et_call"></span>**\_вызов et**  
Значение, соответствующее событию вызова.

<span id="ET_OBJECTCREATION"></span><span id="et_objectcreation"></span>**ET \_ обжекткреатион**  
Значение, соответствующее событию создания объекта.

<span id="ET_OBJECTPOPULATION"></span><span id="et_objectpopulation"></span>**ET \_ обжектпопулатион**  
Значение, соответствующее событию заполнения объекта.

<span id="ET_CALLSYNC"></span><span id="et_callsync"></span>**ET \_ каллсинк**  

<span id="ET_DRAW"></span><span id="et_draw"></span>**\_Рисование et**  
Значение, соответствующее событию вызова Draw.

<span id="ET_DISPATCH"></span><span id="et_dispatch"></span>**\_Диспетчер et**  
Значение, соответствующее событию диспетчеризации.

## <a name="requirements"></a>Требования

<table><colgroup><col  /><col  /></colgroup><tbody><tr class="odd"><td><p>Заголовок</p></td><td>Вспиксенгине. h</td></tr></tbody></table>
