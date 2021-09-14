---
title: Сообщение TVM_MAPHTREEITEMTOACCID (Коммктрл. h)
description: Карты хтриитем к идентификатору специальных возможностей.
ms.assetid: 87ef0785-88c1-49f4-8a05-872577e16fe4
keywords:
- элементы управления Windows сообщений TVM_MAPHTREEITEMTOACCID
topic_type:
- apiref
api_name:
- TVM_MAPHTREEITEMTOACCID
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ad6267c2040583917283fc444db74ddacbdabd69
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165676"
---
# <a name="tvm_maphtreeitemtoaccid-message"></a>\_Сообщение TVM мафтриитемтоакЦид

Карты **хтриитем** к идентификатору специальных возможностей.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>**Хтриитем** , сопоставленный с идентификатором специальных возможностей.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает идентификатор специальных возможностей.

## <a name="remarks"></a>Remarks

При добавлении элемента в элемент управления "дерево" возвращается маркер **хтриитем** , который однозначно определяет элемент.

> [!Note]  
> Чтобы использовать это сообщение, необходимо указать манифест, указывающий Comclt32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_МафтриитемтоакЦид TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_maphtreeitemtoaccid)
</dt> </dl>

 

 





