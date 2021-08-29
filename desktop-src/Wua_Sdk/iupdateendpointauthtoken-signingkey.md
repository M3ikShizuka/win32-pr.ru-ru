---
description: Возвращает ключ, используемый для шифрования исходящих сообщений, которые защищает маркер.
ms.assetid: 1ADBDFC8-E4D9-440B-B310-913213086283
title: 'Метод Иупдатиндпоинтаустокен:: SigningKey (Упдатиндпоинтаус. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IUpdateEndpointAuthToken.SigningKey
api_type:
- COM
api_location:
- UpdateEndpointAuth.dll
ms.openlocfilehash: 45e513483db561ad27e9f1c2f7e18457b039d4bd7eaa1aaa61194443c8ccc78e
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119855744"
---
# <a name="iupdateendpointauthtokensigningkey-method"></a>Метод Иупдатиндпоинтаустокен:: SigningKey

Возвращает ключ, используемый для шифрования исходящих сообщений, которые защищает маркер.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SigningKey(
  [in, out, unique] BYTE  *pbKey,
  [in, out]         ULONG *pcbKeySize
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пбкэй* \[ в, out\]
</dt> <dd>

Ключ, используемый для шифрования исходящих сообщений.

</dd> <dt>

*пкбкэйсизе* \[ в, out\]
</dt> <dd>

Размер ключа, на который ссылается *пбкэй* пареметер.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

При успешном выполнении возвращает значение **\_ ОК** . в противном случае возвращает код ошибки COM или Windows.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP, Windows 2000 Professional с SP3 \[ только для настольных приложений\]<br/>                   |
| Минимальная версия сервера<br/> | Windows сервер 2003, Windows 2000 server с пакетом обновления 3 (SP3), \[ только классические приложения\]<br/>                |
| Заголовок<br/>                   | <dl> <dt>Упдатиндпоинтаус. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Упдатиндпоинтаус. idl</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>Упдатиндпоинтаус. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>UpdateEndpointAuth.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**иупдатиндпоинтаустокен**](iupdateendpointauthtoken.md)
</dt> </dl>

 

 




