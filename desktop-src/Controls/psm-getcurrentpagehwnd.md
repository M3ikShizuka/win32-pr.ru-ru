---
title: Сообщение PSM_GETCURRENTPAGEHWND (Пршт. h)
description: Извлекает маркер окна текущей страницы на странице свойств. Это сообщение можно отправить явным образом или с помощью \_ макроса пропшит жеткуррентпажехвнд.
ms.assetid: 1f2d0af9-5853-48e7-b827-483be032b6ca
keywords:
- элементы управления Windows сообщений PSM_GETCURRENTPAGEHWND
topic_type:
- apiref
api_name:
- PSM_GETCURRENTPAGEHWND
api_location:
- Prsht.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ae9ac89e6bc60317f2caf31ea92754d10983e11a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167576"
---
# <a name="psm_getcurrentpagehwnd-message"></a>\_Сообщение ПСМ жеткуррентпажехвнд

Извлекает маркер окна текущей страницы на странице свойств. Это сообщение можно отправить явным образом или с помощью макроса [**пропшит \_ жеткуррентпажехвнд**](/windows/desktop/api/Prsht/nf-prsht-propsheet_getcurrentpagehwnd) .

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

Возвращает маркер окна текущей страницы свойств.

## <a name="remarks"></a>Remarks

Используйте сообщение **ПСМ \_ жеткуррентпажехвнд** с немодальными страницами свойств, чтобы определить, когда следует уничтожить диалоговое окно. Когда пользователь нажимает кнопку **ОК** или **Отмена** , **ПСМ \_ жеткуррентпажехвнд** возвращает **значение NULL**, а затем можно использовать функцию [**дестройвиндов**](/windows/desktop/api/winuser/nf-winuser-destroywindow) для уничтожения диалогового окна.

> [!Note]  
> Это сообщение не поддерживается при использовании стиля мастера Aero ([**командном PSH \_ аеровизард**](/windows/desktop/api/Prsht/ns-prsht-propsheetheadera_v2)).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Пршт. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Страница свойств**](/windows/desktop/api/Prsht/nf-prsht-propertysheeta)
</dt> </dl>

 

