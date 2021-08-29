---
description: Пропускает указанное число элементов во время перечисления доступных объектов IWiaItem2.
ms.assetid: 7a5e9e1c-1e6e-4de0-9499-bf89e35c19aa
title: 'Метод IEnumWiaItem2:: Skip (WIA. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IEnumWiaItem2.Skip
api_type:
- COM
api_location:
- Wia.h
ms.openlocfilehash: e8676f997ea509bc6a6632a38230b16cf5477ef807f0de25d1505afd462fe834
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119814254"
---
# <a name="ienumwiaitem2skip-method"></a>Метод IEnumWiaItem2:: Skip

Пропускает указанное число элементов во время перечисления доступных объектов [**IWiaItem2**](-wia-iwiaitem2.md) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Skip(
  [in] ULONG cElt
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*cElt* \[ окне\]
</dt> <dd>

Тип: **ulong**

Указывает число пропускаемых элементов.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>WIA. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>WIA. idl</dt> </dl> |



 

 




