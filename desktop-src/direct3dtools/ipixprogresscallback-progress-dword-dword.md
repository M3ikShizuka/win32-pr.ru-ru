---
description: Обратный вызов, уведомляющий узел о ходе выполнения связанного запроса.
MS-HAID: vspixengine.IPixProgressCallback\_Progress\_DWORD\_DWORD
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: 'Ипикспрогресскаллбакк: метод:P рогресс'
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: BE74599B-C98F-4BDB-ACDF-641F77A35EEB
api_name:
- IPixProgressCallback.Progress
api_type:
- COM
api_location:
- vspixengine.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: fbdc28d4ef248b905f39e03e199a08a30b5f92cf
ms.sourcegitcommit: c276a8912787b2cda74dcf54eb96df961bb1188b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2021
ms.locfileid: "122626818"
---
# <a name="span-idvspixengineipixprogresscallback_progress_dword_dwordspanipixprogresscallbackprogress-method"></a><span id="vspixengine.ipixprogresscallback_progress_dword_dword"></span>Ипикспрогресскаллбакк: метод:P рогресс

Обратный вызов, уведомляющий узел о ходе выполнения связанного запроса.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Progress(
   DWORD current,
   DWORD maxSize
);
```

## <a name="parameters"></a>Параметры

*данном*   
Часть запроса завершена в виде количества завершенных шагов.

*maxSize*   
Общее число шагов для выполнения запроса.

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования

<table><colgroup><col  /><col  /></colgroup><tbody><tr class="odd"><td><p>Заголовок</p></td><td>Вспиксенгине. h</td></tr></tbody></table>

## <a name="span-idsee_alsospansee-also"></a><span id="see_also"></span> См. также

[**ипикспрогресскаллбакк**](/windows/desktop/direct3dtools/ipixprogresscallback)

 

 
