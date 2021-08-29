---
title: Сообщение TCM_SETIMAGELIST (Коммктрл. h)
description: Присваивает список изображений элементу управления "Вкладка". Это сообщение можно отправить явным образом или с помощью \_ макроса табктрл сетимажелист.
ms.assetid: b457c73c-4c38-4bc5-af5d-12bbd24504a6
keywords:
- элементы управления Windows сообщений TCM_SETIMAGELIST
topic_type:
- apiref
api_name:
- TCM_SETIMAGELIST
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e3fee54072091f177d1600f81f659b69a2713d4c689c6e1a2e0b05f74777e01e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120104864"
---
# <a name="tcm_setimagelist-message"></a>\_Сообщение СЕТИМАЖЕЛИСТ TCM

Присваивает список изображений элементу управления "Вкладка". Это сообщение можно отправить явным образом или с помощью макроса [**табктрл \_ сетимажелист**](/windows/desktop/api/Commctrl/nf-commctrl-tabctrl_setimagelist) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Обработчик для списка изображений, присваиваемый элементу управления "Вкладка".

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает указатель на предыдущий список изображений или **значение NULL** , если предыдущий список изображений отсутствует.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





