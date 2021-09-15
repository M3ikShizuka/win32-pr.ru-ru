---
description: Определяет, поддерживает ли устройство ввода Мультисенсорная.
ms.assetid: 4fef7060-2235-4bee-a37b-40d827732b30
title: 'Метод ITablet3:: Исмултитауч'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ITablet3.IsMultiTouch
api_type:
- COM
api_location:
- wisptis.exe
- wisptis.exe.dll
ms.openlocfilehash: ed05e110c13af8fe73eebf004183de42eb9fffd7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127579467"
---
# <a name="itablet3ismultitouch-method"></a>Метод ITablet3:: Исмултитауч

Определяет, поддерживает ли устройство ввода Мультисенсорная.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT IsMultiTouch(
  [out] BOOL *bIsMultiTouch
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*бисмултитауч* \[ заполняет\]
</dt> <dd>

Указывает, является ли устройство Мультисенсорная.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **\_ ОК** в случае успеха, в противном случае возвращает код ошибки, например **е \_ Failed**.

## <a name="remarks"></a>Remarks

После определения с помощью [**IRealTimeStylus3:: мултитаученаблед**](/windows/desktop/api/rtscom/nf-rtscom-irealtimestylus3-get_multitouchenabled) или **ITablet3:: исмултитауч** , доступного для Мультисенсорная, приложение может выбрать для Мультисенсорная входных сообщений. Дополнительные сведения о методах фильтрации Мультисенсорная доступны в разделе Свойства **IRealTimeStylus3:: мултитаученаблед** .

## <a name="examples"></a>Примеры


```C++
CComQIPtr<ITablet3> spITablet3 = g_spITablet3;
VARIANT_BOOL b;
spITablet3->get_IsMultiTouch(&b);
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                                |
| Библиотека<br/>                  | <dl> <dt>Wisptis.exe</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ITablet3**](itablet3.md)
</dt> <dt>

[**мултитаученаблед**](/windows/desktop/api/rtscom/nf-rtscom-irealtimestylus3-get_multitouchenabled)
</dt> </dl>

 

 




