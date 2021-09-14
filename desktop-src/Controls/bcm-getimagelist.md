---
title: Сообщение BCM_GETIMAGELIST (Коммктрл. h)
description: Возвращает \_ структуру IMAGELIST, описывающую список изображений, назначенных элементу управления "Кнопка". Это сообщение можно отправить явным образом или воспользоваться макросом "Кнопка" \_ .
ms.assetid: 79383758-53d4-4955-b472-befd338cbec6
keywords:
- элементы управления Windows сообщений BCM_GETIMAGELIST
topic_type:
- apiref
api_name:
- BCM_GETIMAGELIST
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5b0c28e997e23d6df63150fe2283d04be1a8c0d4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170135"
---
# <a name="bcm_getimagelist-message"></a>\_Сообщение BCM ImageList

Возвращает структуру [**\_ IMAGELIST**](/windows/desktop/api/Commctrl/ns-commctrl-button_imagelist) , описывающую список изображений, назначенных элементу управления "Кнопка". Это сообщение можно отправить явным образом или воспользоваться макросом [**"Кнопка" \_**](/windows/desktop/api/Commctrl/nf-commctrl-button_getimagelist) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**\_ IMAGELIST**](/windows/desktop/api/Commctrl/ns-commctrl-button_imagelist) , содержащую сведения о списке изображений.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если сообщение завершается с ошибкой, возвращается **значение true**. В противном случае возвращается **значение false**.

## <a name="remarks"></a>Remarks

> [!Note]  
> Чтобы использовать это сообщение, необходимо указать манифест, указывающий Comclt32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





