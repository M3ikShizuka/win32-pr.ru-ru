---
title: Сообщение TCM_GETROWCOUNT (Коммктрл. h)
description: Извлекает текущее число строк вкладок в элементе управления "Вкладка". Это сообщение можно отправить явно или с помощью \_ макроса табктрл.
ms.assetid: ef104374-1030-46c3-876e-083df73854ab
keywords:
- элементы управления Windows сообщений TCM_GETROWCOUNT
topic_type:
- apiref
api_name:
- TCM_GETROWCOUNT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c9bc3d9985591a08b96be2f21d55b8a6cade9b7a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166252"
---
# <a name="tcm_getrowcount-message"></a>\_Сообщение TCM ROWCOUNT

Извлекает текущее число строк вкладок в элементе управления "Вкладка". Это сообщение можно отправить явно или с помощью макроса [**табктрл \_**](/windows/desktop/api/Commctrl/nf-commctrl-tabctrl_getrowcount) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает число строк вкладок.

## <a name="remarks"></a>Remarks

Только элементы управления "Вкладка", имеющие [**\_ Многострочный стиль TCS**](tab-control-styles.md) , могут содержать несколько строк вкладок.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





