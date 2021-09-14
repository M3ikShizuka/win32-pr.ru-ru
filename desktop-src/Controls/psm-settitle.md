---
title: Сообщение PSM_SETTITLE (Пршт. h)
description: Задает заголовок страницы свойств. Это сообщение можно отправить явным образом или с помощью \_ макроса пропшит сеттитле.
ms.assetid: 53ce8e20-4554-41f4-bad9-fb24c2c93c34
keywords:
- элементы управления Windows сообщений PSM_SETTITLE
topic_type:
- apiref
api_name:
- PSM_SETTITLE
- PSM_SETTITLEA
- PSM_SETTITLEW
api_location:
- Prsht.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1a848a5bdaeaae64b6f1825740d1e8ade07a5a22
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167475"
---
# <a name="psm_settitle-message"></a>\_Сообщение ПСМ сеттитле

Задает заголовок страницы свойств. Это сообщение можно отправить явным образом или с помощью макроса [**пропшит \_ сеттитле**](/windows/desktop/api/Prsht/nf-prsht-propsheet_settitle) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Флаг, указывающий, включать ли префикс "Свойства" или суффикс "Properties" (в зависимости от версии) с указанной строкой заголовка. Если это значение равно КОМАНДНОМ PSH \_ проптитле, то добавляется префикс или суффикс.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на буфер, содержащий строку заголовка. Если [**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85)) этого параметра имеет **значение NULL**, то страница свойств загружает строковый ресурс, указанный в параметре [**ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85)).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

В мастере Aero это сообщение можно использовать для динамического изменения заголовка внутренней страницы. Например, при обработке уведомления [PSN \_ сетактиве](psn-setactive.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Пршт. h</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **ПСМ \_ СЕТТИТЛЕВ** (Юникод) и **ПСМ \_ сеттитлеа** (ANSI)<br/>              |



 

