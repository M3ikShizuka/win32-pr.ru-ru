---
description: Функция обратного вызова, используемая для уведомления узла об ошибках во время записи или воспроизведения.
MS-HAID: vspixengine.IFileIOCallback\_ResultCallback\_DWORD
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: 'Метод Ифилеиокаллбакк:: Ресулткаллбакк'
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: E4418A63-47C6-4F12-94FA-0F1B5465FE84
api_name:
- IFileIOCallback.ResultCallback
api_type:
- COM
api_location:
- vspixengine.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: 29d639a01cd509a6d04432a311ab66ab17e8f5d7
ms.sourcegitcommit: c276a8912787b2cda74dcf54eb96df961bb1188b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2021
ms.locfileid: "122626930"
---
# <a name="span-idvspixengineifileiocallback_resultcallback_dwordspanifileiocallbackresultcallback-method"></a><span id="vspixengine.ifileiocallback_resultcallback_dword"></span>Метод Ифилеиокаллбакк:: Ресулткаллбакк

Функция обратного вызова, используемая для уведомления узла об ошибках во время записи или воспроизведения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT ResultCallback(
   DWORD resultState
);
```

## <a name="parameters"></a>Параметры

*ресултстате*   
Указывает тип обнаруженной ошибки.

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования

<table><colgroup><col  /><col  /></colgroup><tbody><tr class="odd"><td><p>Заголовок</p></td><td>Вспиксенгине. h</td></tr></tbody></table>

## <a name="span-idsee_alsospansee-also"></a><span id="see_also"></span> См. также

[**ифилеиокаллбакк**](/windows/desktop/direct3dtools/ifileiocallback)

 

 
