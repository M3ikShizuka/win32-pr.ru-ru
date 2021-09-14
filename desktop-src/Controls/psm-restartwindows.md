---
title: Сообщение PSM_RESTARTWINDOWS (Пршт. h)
description: указывает, что для вступления изменений в силу необходимо перезапустить Windows.
ms.assetid: 5bf634ee-7408-45df-adb6-c5b947f6c47b
keywords:
- элементы управления Windows сообщений PSM_RESTARTWINDOWS
topic_type:
- apiref
api_name:
- PSM_RESTARTWINDOWS
api_location:
- Prsht.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: eb12126ae0a2b9187a941ccc1aff53186a0cda7d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167516"
---
# <a name="psm_restartwindows-message"></a>\_Сообщение ПСМ рестартвиндовс

указывает, что для вступления изменений в силу необходимо перезапустить Windows.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Должен равняться нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

Приложение должно отправить это сообщение только в ответ на код уведомления [PSN \_ Apply](psn-apply.md) или [PSN \_ киллактиве](psn-killactive.md) . Сообщение **ПСМ \_ рестартвиндовс** можно отправить явным образом или с помощью макроса [**пропшит \_ рестартвиндовс**](/windows/desktop/api/Prsht/nf-prsht-propsheet_restartwindows) .

Это сообщение приводит к тому, что функция [**Страница свойств**](/windows/desktop/api/Prsht/nf-prsht-propertysheeta) ВОЗВРАЩАЕТ \_ значение ID псрестартвиндовс, но только в том случае, если пользователь нажмет кнопку **ОК** , чтобы закрыть страницу свойств. перезапускайте Windows приложения, что можно сделать с помощью функции [**ExitWindowsEx**](/windows/desktop/api/winuser/nf-winuser-exitwindowsex) .

> [!Note]  
> Это сообщение не поддерживается при использовании стиля мастера Aero ([**командном PSH \_ аеровизард**](/windows/desktop/api/Prsht/ns-prsht-propsheetheadera_v2)).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Пршт. h</dt> </dl> |



 

