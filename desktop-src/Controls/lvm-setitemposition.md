---
title: Сообщение LVM_SETITEMPOSITION (Коммктрл. h)
description: Перемещает элемент в указанную позицию в элементе управления "представление списка" (должен быть в виде значка или маленького значка). Это сообщение можно отправить явно или с помощью \_ макроса Сетитемпоситион ListView.
ms.assetid: dfb35af4-e6c3-40fc-9d7c-cf0d68a3ea01
keywords:
- элементы управления Windows сообщений LVM_SETITEMPOSITION
topic_type:
- apiref
api_name:
- LVM_SETITEMPOSITION
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 111f961b668e13fa10fdfb00cdf430aba1bc9d0b1c0b04295e5777a46f5cb9a3
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119915254"
---
# <a name="lvm_setitemposition-message"></a>\_Сообщение LVM сетитемпоситион

Перемещает элемент в указанную позицию в элементе управления "представление списка" (должен быть в виде значка или маленького значка). Это сообщение можно отправить явно или с помощью макроса [**\_ сетитемпоситион ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_setitemposition) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Индекс элемента представления списка.

</dd> <dt>

*lParam* 
</dt> <dd>

[**Ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85)) указывает новую позицию по оси x верхнего левого угла элемента в координатах представления. [**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85)) указывает новую позицию y верхнего левого угла элемента в координатах представления.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="remarks"></a>Remarks

Если элемент управления "список" имеет стиль [**\_ автоупорядочивания LVS**](list-view-window-styles.md) , элементы в элементе управления "список" упорядочиваются после установки позиции элемента.

в Windows Vista отправка этого сообщения в элемент управления "представление списка" с помощью [**стиля \_ автоупорядочивания LVS**](list-view-window-styles.md) ничего не делает, а возвращаемое значение равно **FALSE**.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

