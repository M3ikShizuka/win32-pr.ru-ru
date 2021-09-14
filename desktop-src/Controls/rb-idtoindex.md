---
title: Сообщение RB_IDTOINDEX (Коммктрл. h)
description: Преобразует идентификатор диапазона в индекс диапазона в элементе управления главной панели.
ms.assetid: vs|controls|~\controls\rebar\messages\rb_idtoindex.htm
keywords:
- элементы управления Windows сообщений RB_IDTOINDEX
topic_type:
- apiref
api_name:
- RB_IDTOINDEX
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7c7acd85862bc4787a6b32d2fdd3c897a52913b3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167324"
---
# <a name="rb_idtoindex-message"></a>\_Сообщение ИДТОИНДЕКС RB

Преобразует идентификатор диапазона в индекс диапазона в элементе управления главной панели.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Определяемый приложением идентификатор рассматриваемого диапазона. Это значение, передаваемое члену **WID** структуры [**ребарбандинфо**](/windows/win32/api/commctrl/ns-commctrl-rebarbandinfoa) при вставке полосы.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает индекс полосы с отсчетом от нуля в случае успеха или значение-1 в противном случае. При наличии повторяющихся идентификаторов диапазонов возвращается первый из них.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





