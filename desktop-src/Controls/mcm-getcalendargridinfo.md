---
title: Сообщение MCM_GETCALENDARGRIDINFO (Коммктрл. h)
description: Возвращает сведения о сетке календаря.
ms.assetid: 6b385362-f963-4041-bc9f-d2b7a890c9b4
keywords:
- элементы управления Windows сообщений MCM_GETCALENDARGRIDINFO
topic_type:
- apiref
api_name:
- MCM_GETCALENDARGRIDINFO
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 506f6193ab32d059bb85fa4583441bfbe027f224
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065762"
---
# <a name="mcm_getcalendargridinfo-message"></a>\_Сообщение MCM жеткалендаргридинфо

Возвращает сведения о сетке календаря.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**мкгридинфо**](/windows/win32/api/commctrl/ns-commctrl-mcgridinfo) , содержащую сведения о сетке календаря.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

**Значение true** , если выполнено успешно; в противном случае — **false**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





