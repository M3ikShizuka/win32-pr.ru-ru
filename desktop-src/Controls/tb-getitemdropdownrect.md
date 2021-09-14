---
title: Сообщение TB_GETITEMDROPDOWNRECT (Коммктрл. h)
description: Возвращает ограничивающий прямоугольник раскрывающегося окна для элемента панели инструментов с \_ раскрывающимся списком Style бтнс.
ms.assetid: 4b59c96b-8d75-44c1-b771-c1d62502a2c2
keywords:
- элементы управления Windows сообщений TB_GETITEMDROPDOWNRECT
topic_type:
- apiref
api_name:
- TB_GETITEMDROPDOWNRECT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: dbcbcef725b0ade0bfc776200fa5b191618d2ccb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166799"
---
# <a name="tb_getitemdropdownrect-message"></a>\_Сообщение ЖЕТИТЕМДРОПДОВНРЕКТ ТБ

Возвращает ограничивающий прямоугольник раскрывающегося окна для элемента панели инструментов с [**\_ раскрывающимся списком Style бтнс**](toolbar-control-and-button-styles.md).

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* \[ окне\]
</dt> <dd>

Отсчитываемый от нуля индекс элемента управления ToolBar, для которого требуется получить ограничивающий прямоугольник.

</dd> <dt>

*lParam* \[ в, out\]
</dt> <dd>Указатель на структуру <a href="/previous-versions//dd162897(v=vs.85)">**Rect**</a> для получения сведений о ограничивающем прямоугольнике. Отправитель сообщения отвечает за выделение этой структуры. Координаты, возвращаемые в структуре **Rect** , выражаются как клиентские координаты.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Всегда возвращает ненулевое значение.

## <a name="remarks"></a>Remarks

Элемент должен иметь стиль [**\_ раскрывающегося списка бтнс**](toolbar-control-and-button-styles.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

