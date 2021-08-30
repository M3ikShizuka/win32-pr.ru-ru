---
title: Сообщение UDM_SETPOS (Коммктрл. h)
description: Задает текущую точку для элемента управления "вверх/вниз" с 16-разрядной точностью.
ms.assetid: e7c8b55f-3a4f-47e7-8c7d-e47509f27f1d
keywords:
- элементы управления Windows сообщений UDM_SETPOS
topic_type:
- apiref
api_name:
- UDM_SETPOS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f1f87d079a7bbe454084785cba8ed3361193224edd3e781441f4fe614533b8dd
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120088434"
---
# <a name="udm_setpos-message"></a>\_Сообщение СЕТПОС UDM

Задает текущую точку для элемента управления "вверх/вниз" с 16-разрядной точностью.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Новое расположение элемента управления "вверх/вниз". Если параметр находится за пределами указанного диапазона элемента управления, для свойства *lParam* будет установлено ближайшее допустимое значение.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение является предыдущей позицией.

## <a name="remarks"></a>Remarks

Это сообщение поддерживает только 16-разрядные позиции. Если 32-разрядные значения включены для элемента управления "вверх/вниз" [**с \_ SETRANGE32 UDM**](udm-setrange32.md), [**Используйте \_ SETPOS32 UDM**](udm-setpos32.md).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

**Ссылки**
</dt> <dt>

[**многомерный \_ диапазон UDM**](udm-getrange.md)
</dt> <dt>

[**\_ЖЕТПОС UDM**](udm-getpos.md)
</dt> </dl>

 

 





