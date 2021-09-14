---
description: Уменьшает ссылки на поставщик протокола SSL (SSL).
ms.assetid: 67bfa4b5-c02c-4a76-871d-93f3bf4e3602
title: Функция Сслдекрементпровидерреференцекаунт (Сслпровидер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SslDecrementProviderReferenceCount
api_type:
- DllExport
api_location:
- Ncrypt.dll
ms.openlocfilehash: 4d3fe072c02f22b713115dd5191b0b5e0cedbb37
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067097"
---
# <a name="ssldecrementproviderreferencecount-function"></a>Функция Сслдекрементпровидерреференцекаунт

Функция **сслдекрементпровидерреференцекаунт** уменьшает ссылки на поставщик [*протокола SSL*](/windows/desktop/SecGloss/s-gly) (SSL).

## <a name="syntax"></a>Синтаксис


```C++
SECURITY_STATUS WINAPI SslDecrementProviderReferenceCount(
  _In_ NCRYPT_PROV_HANDLE hSslProvider
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*хсслпровидер* \[ окне\]
</dt> <dd>

Маркер экземпляра поставщика протокола SSL.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если функция завершается с ошибкой, она возвращает ноль.

Если функция завершается ошибкой, она возвращает ненулевое значение ошибки.

Возможные коды возврата включают, но не ограничиваются следующим.



| Возвращаемый код и значение                                                                                                                                                        | Описание                                      |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------|
| <dl> <dt> **\_ Недопустимое \_ состояние**</dt> <dt>0xC0000008L</dt> Handle </dl> | Недопустимый маркер поставщика SSL.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                     |
| Заголовок<br/>                   | <dl> <dt>Сслпровидер. h</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Ncrypt.dll</dt> </dl>    |



 

