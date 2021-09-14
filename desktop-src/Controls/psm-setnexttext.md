---
title: Сообщение PSM_SETNEXTTEXT (Пршт. h)
description: Задает текст кнопки "Далее" в мастере. Это сообщение можно отправить явным образом или с помощью \_ макроса пропшит сетнексттекст.
ms.assetid: 4608425e-1724-4d0b-b0f6-9fec147a85f6
keywords:
- элементы управления Windows сообщений PSM_SETNEXTTEXT
topic_type:
- apiref
api_name:
- PSM_SETNEXTTEXT
- PSM_SETNEXTTEXTW
api_location:
- Prsht.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d781a8d76fca5c1e74bcda452b6ab7e03a32aacc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167479"
---
# <a name="psm_setnexttext-message"></a>\_Сообщение ПСМ сетнексттекст

Задает текст кнопки " **Далее** " в мастере. Это сообщение можно отправить явным образом или с помощью макроса [**пропшит \_ сетнексттекст**](/windows/desktop/api/Prsht/nf-prsht-propsheet_setnexttext) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на буфер, содержащий текст.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет осмысленных возвращаемых значений.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Пршт. h</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **ПСМ \_ СЕТНЕКСТТЕКСТВ** (Юникод)<br/>                                         |



 

 





