---
title: Сообщение TCM_GETEXTENDEDSTYLE (Коммктрл. h)
description: Извлекает расширенные стили, используемые в данный момент для элемента управления "Вкладка". Это сообщение можно отправить явным образом или с помощью \_ макроса табктрл жетекстендедстиле.
ms.assetid: 983ffcbe-0d8d-4686-83de-fc564744390f
keywords:
- элементы управления Windows сообщений TCM_GETEXTENDEDSTYLE
topic_type:
- apiref
api_name:
- TCM_GETEXTENDEDSTYLE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: be5c4618fe039fcd05a73e409f0e8ddd7042694d526f902d432d2513bbef96e4
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119876574"
---
# <a name="tcm_getextendedstyle-message"></a>\_Сообщение ЖЕТЕКСТЕНДЕДСТИЛЕ TCM

Извлекает расширенные стили, используемые в данный момент для элемента управления "Вкладка". Это сообщение можно отправить явным образом или с помощью макроса [**табктрл \_ жетекстендедстиле**](/windows/desktop/api/Commctrl/nf-commctrl-tabctrl_getextendedstyle) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **типа DWORD** , представляющее расширенные стили, используемые в данный момент для элемента управления "Вкладка". Это значение представляет собой сочетание [расширенных стилей](tab-control-extended-styles.md)элемента управления Tab.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_СЕТЕКСТЕНДЕДСТИЛЕ TCM**](tcm-setextendedstyle.md)
</dt> </dl>

 

 





