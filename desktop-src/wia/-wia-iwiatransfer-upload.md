---
description: Инициирует отправку данных одного элемента от вызывающего.
ms.assetid: 301ac5d9-b864-4c3c-bd4b-143cc4032dcb
title: 'метод ивиатрансфер:: Upload (Wia. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IWiaTransfer.Upload
api_type:
- COM
api_location:
- Wiaguid.lib
- Wiaguid.dll
ms.openlocfilehash: 6aae6ca8f86d07ec052fdd59d24b0da2b96599d7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362805"
---
# <a name="iwiatransferupload-method"></a>метод ивиатрансфер:: Upload

Инициирует отправку данных одного элемента от вызывающего.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Upload(
  [in] LONG                 lFlags,
  [in] IStream              *pSource,
  [in] IWiaTransferCallback *pIWiaTransferCallback
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*лфлагс* \[ окне\]
</dt> <dd>

Тип: **Long**

В настоящее время не используется. Значение должно быть равно нулю.

</dd> <dt>

*псаурце* \[ окне\]
</dt> <dd>

Тип: **[IStream](/windows/win32/api/objidl/nn-objidl-istream)\***

Указывает указатель на данные [IStream](/windows/win32/api/objidl/nn-objidl-istream) .

</dd> <dt>

*пивиатрансферкаллбакк* \[ окне\]
</dt> <dd>

Тип: **[ **ивиатрансферкаллбакк**](-wia-iwiatransfercallback.md)\***

Указывает указатель на интерфейс [**ивиатрансферкаллбакк**](-wia-iwiatransfercallback.md) вызывающего объекта.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                   |
| Заголовок<br/>                   | <dl> <dt>WIA. h</dt> </dl>       |
| IDL<br/>                      | <dl> <dt>WIA. idl</dt> </dl>     |
| Библиотека<br/>                  | <dl> <dt>Виагуид. lib</dt> </dl> |



 

 
