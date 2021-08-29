---
title: Сообщение TCM_HIGHLIGHTITEM (Коммктрл. h)
description: Задает состояние выделения элемента вкладки. Это сообщение можно отправить явным образом или с помощью \_ макроса табктрл хигхлигхтитем.
ms.assetid: b0d0850a-62d9-46a1-8846-81f67a886ea8
keywords:
- элементы управления Windows сообщений TCM_HIGHLIGHTITEM
topic_type:
- apiref
api_name:
- TCM_HIGHLIGHTITEM
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b355b1a0ad4d228fc8f67051497b0327885f7cafc3860af9c74bac0812b344ab
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119876514"
---
# <a name="tcm_highlightitem-message"></a>\_Сообщение ХИГХЛИГХТИТЕМ TCM

Задает состояние выделения элемента вкладки. Это сообщение можно отправить явным образом или с помощью макроса [**табктрл \_ хигхлигхтитем**](/windows/desktop/api/Commctrl/nf-commctrl-tabctrl_highlightitem) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Значение **типа int** , указывающее Отсчитываемый от нуля индекс элемента управления вкладки.

</dd> <dt>

*lParam* 
</dt> <dd>

[**Ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85)) — это **логическое** значение, определяющее выделенное состояние выделения. Если это значение равно **true**, вкладка выделена; Если **значение равно false**, то для вкладки задано состояние по умолчанию. [**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85)) должен быть равен нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ненулевое значение в случае успеха или ноль в противном случае.

## <a name="remarks"></a>Remarks

В Comctl32.dll версии 6,0 это сообщение не отображается, если тема активна.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

