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
ms.openlocfilehash: ce923feaec893e6f4304eb0b993de33dc1fe2a97
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166783"
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

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

