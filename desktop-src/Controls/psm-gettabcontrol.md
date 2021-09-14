---
title: Сообщение PSM_GETTABCONTROL (Пршт. h)
description: Получает маркер для элемента управления вкладки страницы свойств. Это сообщение можно отправить явно или с помощью \_ макроса пропшит.
ms.assetid: 5ddea541-c8e0-4357-b08e-3b5e64be377f
keywords:
- элементы управления Windows сообщений PSM_GETTABCONTROL
topic_type:
- apiref
api_name:
- PSM_GETTABCONTROL
api_location:
- Prsht.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ab296159cac4dbfb4ef894d90d31bcd74d6ca2e1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167571"
---
# <a name="psm_gettabcontrol-message"></a>Сообщение ПСМ в \_ TabControl

Получает маркер для элемента управления вкладки страницы свойств. Это сообщение можно отправить явно или с помощью макроса [**пропшит \_**](/windows/desktop/api/Prsht/nf-prsht-propsheet_gettabcontrol) .

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

Возвращает маркер для элемента управления "Вкладка".

## <a name="remarks"></a>Remarks

> [!Note]  
> Это сообщение не поддерживается при использовании стиля мастера Aero ([**командном PSH \_ аеровизард**](/windows/desktop/api/Prsht/ns-prsht-propsheetheadera_v2)).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Пршт. h</dt> </dl> |



 

 





