---
title: Сообщение CCM_DPISCALE (Коммктрл. h)
description: Включает автоматическое масштабирование с высоким числом точек на дюйм в элементах управления Tree-View, List-View элементах управления, элементах управления ComboBoxEx, элементах управления "заголовок", кнопках, элементах управления ToolBar, анимации и списках изображений.
ms.assetid: 3c751f10-992c-41f8-8f0b-3dc58f0591e4
keywords:
- элементы управления Windows сообщений CCM_DPISCALE
topic_type:
- apiref
api_name:
- CCM_DPISCALE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 56ef978f486f370adf9872d28e1accbacc37a6de
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145257"
---
# <a name="ccm_dpiscale-message"></a>\_Сообщение ДПИСКАЛЕ CCM

Включает автоматическое масштабирование с высоким числом точек на дюйм в [древовидном представлении](tree-view-controls.md), [элементах управления "представление списка](list-view-control-reference.md)", [элементах](comboboxex-controls.md)управления "ComboBoxEx", [элементах управления "заголовок](header-controls.md)", [кнопках](buttons.md), [элементах управления ToolBar](toolbar-controls-overview.md), [элементах управления анимации](animation-control-overview.md)и [списках изображений](image-lists.md).

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Задайте значение **true**.

</dd> <dt>

*lParam* 
</dt> <dd>

Должен равняться нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение не используется.

## <a name="remarks"></a>Remarks

Для быстрого запуска и [панели задач](/windows/desktop/shell/taskbar) не следует указывать масштабирование DPI, так как изображения уже масштабируются.

Любой элемент управления, использующий список изображений, созданный с помощью метрики маленькие значки, не должен масштабировать свои значки.

> [!Note]  
> Чтобы использовать этот API, необходимо предоставить манифест, указывающий Comclt32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

