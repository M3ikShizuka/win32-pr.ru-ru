---
title: Сообщение TB_AUTOSIZE (Коммктрл. h)
description: Приводит к изменению размера панели инструментов.
ms.assetid: 11aff184-6f18-43a2-9bdc-462fc5ba1680
keywords:
- элементы управления Windows сообщений TB_AUTOSIZE
topic_type:
- apiref
api_name:
- TB_AUTOSIZE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e5f901463888338fd9cadf67472232efe9a25f29
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166904"
---
# <a name="tb_autosize-message"></a>Размер \_ сообщения AUTOSIZE для ТБ

Приводит к изменению размера панели инструментов.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

Приложение отправляет сообщение **\_ AUTOSIZE** по размеру ТБ после изменения размера панели инструментов либо путем установки размера кнопки или растрового изображения, либо путем добавления строк в первый раз.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





