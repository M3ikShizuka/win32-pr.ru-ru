---
description: Обратный вызов, уведомляющий узел о сообщениях, возвращенных связанным запросом.
MS-HAID: vspixengine.IPixErrorCallback\_MessagesCallback\_DWORD\_Issue\_arr
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: 'Метод Ипиксерроркаллбакк:: Мессажескаллбакк'
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: 55343F63-BB58-4F57-884D-CEFE8AB57A27
api_name:
- IPixErrorCallback.MessagesCallback
api_type:
- COM
api_location:
- vspixengine.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: 5dcdf4ea6de43ee0057de13b2feb69a9cf86374d
ms.sourcegitcommit: c276a8912787b2cda74dcf54eb96df961bb1188b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2021
ms.locfileid: "122623890"
---
# <a name="span-idvspixengineipixerrorcallback_messagescallback_dword_issue_arrspanipixerrorcallbackmessagescallback-method"></a><span id="vspixengine.ipixerrorcallback_messagescallback_dword_issue_arr"></span>Метод Ипиксерроркаллбакк:: Мессажескаллбакк

Обратный вызов, уведомляющий узел о сообщениях, возвращенных связанным запросом.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT MessagesCallback(
   DWORD    count,
   Issue [] count0_messages
);
```

## <a name="parameters"></a>Параметры

*расчета*   
Число сообщений.

*\_сообщения count0*   
Сообщения.

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования

<table><colgroup><col  /><col  /></colgroup><tbody><tr class="odd"><td><p>Заголовок</p></td><td>Вспиксенгине. h</td></tr></tbody></table>

## <a name="span-idsee_alsospansee-also"></a><span id="see_also"></span> См. также

[**ипиксерроркаллбакк**](/windows/desktop/direct3dtools/ipixerrorcallback)

 

 
