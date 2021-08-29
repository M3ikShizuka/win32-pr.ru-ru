---
title: Сообщение TCM_GETIMAGELIST (Коммктрл. h)
description: Извлекает список изображений, связанных с элементом управления "Вкладка". Это сообщение можно отправить явно или с помощью \_ макроса табктрлs.
ms.assetid: 86a0d8c7-ff3d-4e16-994e-4c72d1e62e9f
keywords:
- элементы управления Windows сообщений TCM_GETIMAGELIST
topic_type:
- apiref
api_name:
- TCM_GETIMAGELIST
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 17a8c91e5e88397ed436ae14c3500aadd6e450a14d168d1f6bb874c12b24da69
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120104894"
---
# <a name="tcm_getimagelist-message"></a>Сообщение TCM. \_ ImageList

Извлекает список изображений, связанных с элементом управления "Вкладка". Это сообщение можно отправить явно или с помощью макроса [**табктрлs \_**](/windows/desktop/api/Commctrl/nf-commctrl-tabctrl_getimagelist) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает маркер в список изображений в случае успеха или **значение NULL** в противном случае.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





