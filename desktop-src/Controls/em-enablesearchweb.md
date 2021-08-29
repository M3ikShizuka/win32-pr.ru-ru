---
title: Сообщение EM_ENABLESEARCHWEB (Коммктрл. h)
description: Включает или отключает функцию "Поиск в Интернете" и запись в контекстном меню.
ms.assetid: 9393f03e-0719-458b-8122-616df738c417
keywords:
- элементы управления Windows сообщений EM_ENABLESEARCHWEB
topic_type:
- apiref
api_name:
- EM_ENABLESEARCHWEB
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 33cc76e81db5ea7c5b596e0876cad4cfabecc41b5bae62d4a666be3727b38725
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119915864"
---
# <a name="em_enablesearchweb-message"></a>\_Сообщение ЕНАБЛЕСЕАРЧВЕБ EM

Включает или отключает функцию "Поиск в Интернете" и запись в контекстном меню.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Значение **true** указывает, что функция "Поиск в Интернете" включена, а значение " **ложь** " означает, что она отключена.

</dd> <dt>

*lParam* 
</dt> <dd>

Этот параметр не используется.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение не возвращает значение.

## <a name="remarks"></a>Remarks

Если отключить "Поиск в Интернете" с помощью этого сообщения, сообщение [**EM \_ сеарчвеб**](em-searchweb.md) не будет действовать.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, \[ только классические приложения 1809\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2019\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[**EM \_ сеарчвеб**](em-searchweb.md)
</dt> </dl>

 

 





