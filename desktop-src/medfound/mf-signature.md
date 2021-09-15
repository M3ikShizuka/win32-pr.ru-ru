---
description: Содержит сигнатуру глобального списка отзыва (GRL).
ms.assetid: 388a901c-6202-41cf-9c3d-f29d8ccca76b
title: Структура MF_SIGNATURE
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- MF_SIGNATURE
api_type:
- NA
api_location: ''
ms.openlocfilehash: 4827fea8e4259609cbb54f2b58a3d1c88ad6c23e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462081"
---
# <a name="mf_signature-structure"></a>\_Структура сигнатуры MF

Содержит сигнатуру глобального списка отзыва (GRL).

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _MF_SIGNATURE {
  DWORD dwSignVer;
  DWORD cbSign;
  BYTE  rgSign[1];
} MF_SIGNATURE;
```



## <a name="members"></a>Участники

<dl> <dt>

**двсигнвер**
</dt> <dd>

Номер версии сигнатуры.

</dd> <dt>

**кбсигн**
</dt> <dd>

Размер подписи в байтах.

</dd> <dt>

**ргсигн**
</dt> <dd>

Массив байтов размера **кбсигн** , который содержит сигнатуру. Фактический размер массива превышает размер, заданный в объявлении структуры.

</dd> </dl>

## <a name="remarks"></a>Remarks

Эта структура не объявлена в заголовке пакета SDK. Чтобы использовать эту структуру, добавьте приведенное здесь объявление в исходный код.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Отзыв сертификата ОПМ](opm-certificate-revocation.md)
</dt> <dt>

[Структуры ОПМ](opm-structures.md)
</dt> </dl>

 

 




