---
title: Сообщение TVM_MAPACCIDTOHTREEITEM (Коммктрл. h)
description: Карты идентификатор специальных возможностей для хтриитем.
ms.assetid: f4feb7cb-2138-4930-b8ee-b9e2d4b19001
keywords:
- элементы управления Windows сообщений TVM_MAPACCIDTOHTREEITEM
topic_type:
- apiref
api_name:
- TVM_MAPACCIDTOHTREEITEM
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b827b18387723fe4792321f7932e1abb3673466e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165680"
---
# <a name="tvm_mapaccidtohtreeitem-message"></a>\_Сообщение TVM мапакЦидтохтриитем

Карты идентификатор специальных возможностей для **хтриитем**.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>**Uint** , содержащий идентификатор доступа, сопоставляемый с **хтриитем**. </dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **хтриитем** , с которым СОПОСТАВЛЕН указанный идентификатор доступа.

## <a name="remarks"></a>Remarks

При добавлении элемента в элемент управления представлением в виде дерева возвращается **хтриитем** , который однозначно определяет элемент.

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

[**\_МапакЦидтохтриитем TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_mapaccidtohtreeitem)
</dt> </dl>

 

 





