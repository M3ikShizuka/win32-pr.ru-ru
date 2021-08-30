---
description: Представляет сведения о триггере эксперимента.
MS-HAID: vspixengine.ExperimentTrigger
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: Структура Експерименттригжер
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: 3CAA67E5-9C43-4BCD-9388-63EF06AB1C0E
api_name:
- ExperimentTrigger
api_type:
- HeaderDef
api_location:
- vspixengine.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: ce4087e4e4ef30cedeb356730a0a7ae94252d4f3
ms.sourcegitcommit: c276a8912787b2cda74dcf54eb96df961bb1188b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2021
ms.locfileid: "122625180"
---
# <a name="span-idvspixengineexperimenttriggerspanexperimenttrigger-structure"></a><span id="vspixengine.experimenttrigger"></span>Структура Експерименттригжер

Представляет сведения о триггере эксперимента.

## <a name="syntax"></a>Синтаксис


```C++
} ExperimentTrigger;
```

## <a name="members"></a>Участники

**type**  
Тип запуска эксперимента (захват).

**key**  
Если тип равен ЕКСПЕРИМЕНТТРИГЖЕРТИПЕ:: KEY, ключ, используемый для активации захвата.

**фраменумбер**  
Если тип равен ЕКСПЕРИМЕНТТРИГЖЕРТИПЕ:: ФРАМЕНУМБЕР, то номер кадра, который запустит захват.

**каптурекаунт**  
Число последовательных кадров для записи.

**актиониид**  
Идентификатор события действия (снимок экрана, запись кадра и т. д.).

**актионплайлоад**  
Указатель на полезные данные события действия.

## <a name="requirements"></a>Требования

<table><colgroup><col  /><col  /></colgroup><tbody><tr class="odd"><td><p>Заголовок</p></td><td>Вспиксенгине. h</td></tr></tbody></table>

 

 



