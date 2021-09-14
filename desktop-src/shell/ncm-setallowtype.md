---
description: Задает типы сетевых адресов, принимаемые указанным элементом управления для сетевых адресов.
title: Сообщение NCM_SETALLOWTYPE (Шеллапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: FD998452-047A-4aea-A08E-8F6F8C30115B
api_name:
- NCM_SETALLOWTYPE
api_type:
- HeaderDef
api_location:
- Shellapi.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: d9cc822e07022a01439fbe7e41243bd1b78e636b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127346351"
---
# <a name="ncm_setallowtype-message"></a>\_Сообщение НКМ сеталловтипе

Задает типы сетевых адресов, принимаемые указанным элементом управления для сетевых адресов.


```C++
NCM_SETALLOWTYPE

    wParam = (WPARAM) (DWORD) addrMask;

    lParam = 0;            

            
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*аддрмаск* \[ окне\]
</dt> <dd>Указывает типы сетевых адресов в виде одной или нескольких констант типа "сеть — <a href="net-string.md">**\_ строка**</a> ".</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ значение ОК, если успешно, или в противном случае.

## <a name="remarks"></a>Remarks

Набор масок — это критерий, используемый для проверки сетевого адреса в сообщении [**НКМ- \_ Address**](ncm-getaddress.md) .

Это сообщение используется только для управления сетевыми адресами. Чтобы создать экземпляр, используйте класс **мсктлс \_ нетаддресс** , определенный в шеллапи. h. Вызовите [**инитнетворкаддрессконтрол**](/windows/desktop/api/Shellapi/nf-shellapi-initnetworkaddresscontrol) во время выполнения перед отправкой этого сообщения. Будет инициализирована библиотека общих элементов управления, содержащая элемент управления "сетевой адрес".

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Шеллапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**НКМ \_ жеталловтипе**](ncm-getallowtype.md)
</dt> <dt>

[**Нетаддр \_ сеталловтипе**](/windows/desktop/api/Shellapi/nf-shellapi-netaddr_setallowtype)
</dt> </dl>

 

 




