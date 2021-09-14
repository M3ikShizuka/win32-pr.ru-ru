---
title: Сообщение STM_SETICON (Winuser. h)
description: Приложение отправляет \_ сообщение STM сетикон, чтобы связать значок с элементом управления "значок".
ms.assetid: 105b0667-8e23-47ed-9fb1-0792a22d7100
keywords:
- элементы управления Windows сообщений STM_SETICON
topic_type:
- apiref
api_name:
- STM_SETICON
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: cb9c7e2a007c1f866a1c73b3a1c1a55b157add47
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167000"
---
# <a name="stm_seticon-message"></a>\_Сообщение СЕТИКОН STM

Приложение отправляет сообщение **STM \_ сетикон** , чтобы связать значок с элементом управления "значок".

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Обработчик значка, связываемый с элементом управления "значок".

</dd> <dt>

*lParam* 
</dt> <dd>

Этот параметр не используется.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение является обработчиком значка, ранее связанного с элементом управления "значок", или нулем в случае возникновения ошибки.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылка**
</dt> <dt>

[**\_значок STM**](stm-geticon.md)
</dt> <dt>

**Другие ресурсы**
</dt> <dt>

[**лоадикон**](/windows/desktop/api/winuser/nf-winuser-loadicona)
</dt> </dl>

 

