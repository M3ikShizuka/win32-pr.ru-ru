---
title: Сообщение TTM_UPDATETIPTEXT (Коммктрл. h)
description: Задает текст подсказки для инструмента.
ms.assetid: 2a7432dd-76f9-42b4-b639-178dce1d89ef
keywords:
- элементы управления Windows сообщений TTM_UPDATETIPTEXT
topic_type:
- apiref
api_name:
- TTM_UPDATETIPTEXT
- TTM_UPDATETIPTEXTA
- TTM_UPDATETIPTEXTW
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f6c94b14ec83c190ce019ecba1413d2fa05f0103
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165824"
---
# <a name="ttm_updatetiptext-message"></a>\_Сообщение ТТМ упдатетиптекст

Задает текст подсказки для инструмента.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**тулинфо**](/windows/win32/api/commctrl/ns-commctrl-tttoolinfoa) . Члены **хинст** и **лпсзтекст** должны задавать обработчик экземпляра и адрес текста. Элементы **HWND** и **uId** указывают средство для обновления. Перед отправкой этого сообщения необходимо заполнить элемент **кбсизе** этой структуры.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **ТТМ \_ УПДАТЕТИПТЕКСТВ** (Юникод) и **ТТМ \_ упдатетиптекста** (ANSI)<br/>       |



 

 





