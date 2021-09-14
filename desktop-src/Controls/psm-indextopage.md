---
title: Сообщение PSM_INDEXTOPAGE (Пршт. h)
description: Принимает индекс страницы свойств и возвращает его обработчик ХПРОПШИТПАЖЕ. Это сообщение можно отправить явным образом или использовать макрос Пропшит \_ индекстопаже.
ms.assetid: b14b35ad-bae0-4461-a90f-e2bc5e2ccfc2
keywords:
- элементы управления Windows сообщений PSM_INDEXTOPAGE
topic_type:
- apiref
api_name:
- PSM_INDEXTOPAGE
api_location:
- Prsht.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 38f7a5658dbd92f4208e084f1df47a4dc3582156
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167555"
---
# <a name="psm_indextopage-message"></a>\_Сообщение ПСМ индекстопаже

Принимает индекс страницы свойств и возвращает его обработчик ХПРОПШИТПАЖЕ. Это сообщение можно отправить явным образом или использовать макрос [**пропшит \_ индекстопаже**](/windows/desktop/api/Prsht/nf-prsht-propsheet_indextopage) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Отсчитываемый от нуля индекс страницы.

</dd> <dt>

*lParam* 
</dt> <dd>

Должен равняться нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает маркер ХПРОПШИТПАЖЕ страницы свойств, указанный параметром *wParam* в случае успеха. В противном случае возвращается ноль.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Пршт. h</dt> </dl> |



 

 





