---
title: Метод дешифровки Ивмсекуребуффер (Вмдрмсдк. h)
description: Метод дешифровки расшифровывает указатель данных, который был зашифрован путем вызова метода Encrypt.
ms.assetid: 15cedb56-686a-4a3c-81a5-b1797cfe0838
keywords:
- Расшифровка метода Windows Media Format
- Метод расшифровки формата Windows Media Format, интерфейс Ивмсекуребуффер
- Интерфейс Ивмсекуребуффер интерфейса Windows Media Format, метод дешифрации
topic_type:
- apiref
api_name:
- IWMSecureBuffer.Decrypt
api_location:
- Wmdrmsdk.lib
- Wmdrmsdk.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a6f48ae389090840e085c90b0bc5444e7cd6784e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127267120"
---
# <a name="iwmsecurebufferdecrypt-method"></a>Ивмсекуребуффер: метод:D екрипт

Метод **дешифровки** расшифровывает указатель данных, который был зашифрован путем вызова метода [**Encrypt**](iwmsecurebuffer-encrypt.md) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Decrypt(
  [in] IWMSecureChannel *pSecureChannel
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*псекуречаннел* \[ окне\]
</dt> <dd>

Указатель на интерфейс безопасного канала, содержащий указатель зашифрованных данных.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает **значение HRESULT**. Допустимые значения включают, но не ограничиваются, значения, приведенные в следующей таблице.



| Код возврата                                                                          | Описание                      |
|--------------------------------------------------------------------------------------|----------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl> | Метод выполнен успешно.<br/> |



 

## <a name="remarks"></a>Remarks

Нет.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Вмдрмсдк. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>Вмдрмсдк. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Шифрования**](iwmsecurebuffer-encrypt.md)
</dt> <dt>

[**Интерфейс Ивмсекуребуффер**](iwmsecurebuffer.md)
</dt> </dl>

 

 





