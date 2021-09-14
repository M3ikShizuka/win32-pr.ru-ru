---
title: Сообщение LVM_GETGROUPMETRICS (Коммктрл. h)
description: Возвращает сведения о отображении групп.
ms.assetid: 75e7da66-50c6-4834-ae66-e43b8f9b0b34
keywords:
- элементы управления Windows сообщений LVM_GETGROUPMETRICS
topic_type:
- apiref
api_name:
- LVM_GETGROUPMETRICS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c5af8ec50fe74ab90a0f3e44a69e2cbc7dda583e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054087"
---
# <a name="lvm_getgroupmetrics-message"></a>\_Сообщение LVM жетграупметрикс

Возвращает сведения о отображении групп.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен иметь **значение NULL**.</dd> <dt>

*lParam* 
</dt> <dd>Указатель на структуру <a href="/windows/win32/api/commctrl/ns-commctrl-lvgroupmetrics">**лвграупметрикс**</a> , которая получает извлеченные метрики.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение не используется.

## <a name="remarks"></a>Комментарии

> [!Note]  
> Чтобы использовать это сообщение, необходимо указать манифест, указывающий Comclt32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





