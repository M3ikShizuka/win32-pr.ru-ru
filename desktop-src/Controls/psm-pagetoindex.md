---
title: Сообщение PSM_PAGETOINDEX (Пршт. h)
description: Принимает маркер ХПРОПШИТПАЖЕ страницы свойств и возвращает индекс, начинающийся с нуля. Это сообщение можно отправить явным образом или использовать макрос Пропшит \_ пажетоиндекс.
ms.assetid: vs|controls|~\controls\propsheet\messages\psm_pagetoindex.htm
keywords:
- элементы управления Windows сообщений PSM_PAGETOINDEX
topic_type:
- apiref
api_name:
- PSM_PAGETOINDEX
api_location:
- Prsht.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 71651853d0d403c25a0f8c554bd31c2ae649bcf0258b6f1f578a03cc65a3b539
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119985673"
---
# <a name="psm_pagetoindex-message"></a>\_Сообщение ПСМ пажетоиндекс

Принимает маркер ХПРОПШИТПАЖЕ страницы свойств и возвращает индекс, начинающийся с нуля. Это сообщение можно отправить явным образом или использовать макрос [**пропшит \_ пажетоиндекс**](/windows/desktop/api/Prsht/nf-prsht-propsheet_pagetoindex) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

ХПРОПШИТПАЖЕ маркер на страницу свойств.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает отсчитываемый от нуля индекс страницы вкладки свойств, указанной параметром *lParam* в случае успеха. Иначе возвращается значение -1.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Пршт. h</dt> </dl> |



 

 





