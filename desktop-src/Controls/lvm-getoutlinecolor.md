---
title: Сообщение LVM_GETOUTLINECOLOR (Коммктрл. h)
description: Получает цвет границы элемента управления "представление списка", если \_ \_ установлен расширенный стиль окна LVS ex бордерселект.
ms.assetid: cc9d69d1-1470-4eaa-8d54-e31b796cf685
keywords:
- элементы управления Windows сообщений LVM_GETOUTLINECOLOR
topic_type:
- apiref
api_name:
- LVM_GETOUTLINECOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 489f21f2f6d4dcca2c79d92a13a85d7718a85693
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126972090"
---
# <a name="lvm_getoutlinecolor-message"></a>\_Сообщение LVM жетаутлинеколор

Получает цвет границы элемента управления "представление списка", если установлен расширенный стиль окна [**LVS \_ ex \_ бордерселект**](extended-list-view-styles.md) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает структуру **COLORREF** , содержащую цвет границы элемента управления "представление списка".

## <a name="remarks"></a>Комментарии

> [!Note]  
> Чтобы использовать это сообщение, необходимо указать манифест, указывающий Comclt32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





