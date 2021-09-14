---
title: Сообщение PSM_INDEXTOID (Пршт. h)
description: Принимает индекс страницы свойств и возвращает идентификатор ресурса. Это сообщение можно отправить явным образом или использовать макрос Пропшит \_ индекстоид.
ms.assetid: c153675a-360f-4916-aa0b-500636dd9022
keywords:
- элементы управления Windows сообщений PSM_INDEXTOID
topic_type:
- apiref
api_name:
- PSM_INDEXTOID
api_location:
- Prsht.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 643861ecb6dc11d949483defc282d6d65648bdca
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167552"
---
# <a name="psm_indextoid-message"></a>\_Сообщение ПСМ индекстоид

Принимает индекс страницы свойств и возвращает идентификатор ресурса. Это сообщение можно отправить явным образом или использовать макрос [**пропшит \_ индекстоид**](/windows/desktop/api/Prsht/nf-prsht-propsheet_indextoid) .

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

Возвращает идентификатор ресурса страницы свойств, указанной параметром *wParam* в случае успеха. В противном случае возвращается ноль.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Пршт. h</dt> </dl> |



 

 





