---
title: Сообщение TB_GETOBJECT (Коммктрл. h)
description: Получает интерфейс IDropTarget для элемента управления ToolBar.
ms.assetid: b26394ea-6f0f-4084-956d-f9166cc54b76
keywords:
- элементы управления Windows сообщений TB_GETOBJECT
topic_type:
- apiref
api_name:
- TB_GETOBJECT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4671c3b6998c170f6ef59e8a0019b58a166728d1c560eac8420dbaf40c4dcb0f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120061344"
---
# <a name="tb_getobject-message"></a>\_Сообщение об ОБЪЕКТЕ ТБ

Получает [**интерфейс IDropTarget**](/windows/desktop/api/oleidl/nn-oleidl-idroptarget) для элемента управления ToolBar.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Идентификатор запрашиваемого интерфейса. Это значение должно указывать на **IID \_ интерфейс IDropTarget**.

</dd> <dt>

*lParam* 
</dt> <dd>

Адрес, получающий указатель интерфейса. При возникновении ошибки в этот адрес помещается **пустой** указатель.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** , указывающее на успешное выполнение или сбой операции.

## <a name="remarks"></a>Remarks

Панель инструментов [**интерфейс IDropTarget**](/windows/desktop/api/oleidl/nn-oleidl-idroptarget) используется панелью инструментов, когда объекты перетаскиваются на него или отбрасываются.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

