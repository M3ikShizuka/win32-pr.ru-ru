---
title: Сообщение LM_SETITEM (Коммктрл. h)
description: Задает состояния и атрибуты элемента.
ms.assetid: 02a68a31-2541-480e-b768-449d40e5e9e0
keywords:
- элементы управления Windows сообщений LM_SETITEM
topic_type:
- apiref
api_name:
- LM_SETITEM
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 11888a76b11ccec7e8e659ca3a33bb23a71667ee
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126972130"
---
# <a name="lm_setitem-message"></a>\_Сообщение СЕТИТЕМ LM

Задает состояния и атрибуты элемента.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен иметь **значение NULL**. </dd> <dt>

*lParam* 
</dt> <dd>Указатель на структуру <a href="/windows/win32/api/commctrl/ns-commctrl-litem">литем</a> , содержащую новые состояния и атрибуты, необходимые для ссылки. </dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если сообщение завершается с ошибкой при установке указанных значений и атрибутов.

## <a name="remarks"></a>Комментарии

С сообщением [**LM- \_ Item**](lm-getitem.md) можно получить доступ к ссылкам только через числовой индекс, возвращенный в **iLink** члене [**литем**](/windows/win32/api/commctrl/ns-commctrl-litem). Обращение по ссылке через имя идентификатора, возвращенное в **сзид** , не поддерживается.

> [!Note]  
> Чтобы использовать это сообщение, необходимо указать манифест, указывающий Comctl32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





