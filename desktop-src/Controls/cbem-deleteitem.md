---
title: Сообщение CBEM_DELETEITEM (Коммктрл. h)
description: Удаляет элемент из элемента управления ComboBoxEx.
ms.assetid: 688cf388-54ba-4b45-88d7-628da49d8615
keywords:
- элементы управления Windows сообщений CBEM_DELETEITEM
topic_type:
- apiref
api_name:
- CBEM_DELETEITEM
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: afba180ad6b714b597fe688cbaf1496b92735d8924cd6a238d56f081753fb3e2
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120063313"
---
# <a name="cbem_deleteitem-message"></a>\_Сообщение кбем DELETEITEM

Удаляет элемент из элемента управления ComboBoxEx.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Отсчитываемый от нуля индекс удаляемого элемента.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение типа INT, представляющее количество элементов, остающихся в элементе управления. Если *ииндекс* является недопустимым, сообщение ВОЗВРАЩАЕТ значение CB \_ Err.

## <a name="remarks"></a>Remarks

Это сообщение сопоставляется с полем со списком элемент управления "сообщение [**CB \_ делетестринг**](cb-deletestring.md)".

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





