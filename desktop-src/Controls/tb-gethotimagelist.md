---
title: Сообщение TB_GETHOTIMAGELIST (Коммктрл. h)
description: Извлекает список изображений, используемый элементом управления Toolbar для показа кнопок.
ms.assetid: 63054449-2768-459c-933c-781d31bdcc15
keywords:
- элементы управления Windows сообщений TB_GETHOTIMAGELIST
topic_type:
- apiref
api_name:
- TB_GETHOTIMAGELIST
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9e19c1f3989b0d749a9c663d00b5fb7b54d67fc0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166827"
---
# <a name="tb_gethotimagelist-message"></a>\_Сообщение ЖЕСОТИМАЖЕЛИСТ ТБ

Извлекает список изображений, используемый элементом управления Toolbar для показа кнопок.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает указатель на список изображений, используемый элементом управления для показа активных кнопок, или **значение NULL** , если список горячих образов не задан.

## <a name="remarks"></a>Remarks

Кнопка находится в активном положении при наведении на нее курсора. Элементы управления "панель инструментов" должны иметь [**стиль \_ списка**](toolbar-control-and-button-styles.md) [**тбстиле \_ Flat**](toolbar-control-and-button-styles.md) или тбстиле, чтобы иметь активные элементы.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





