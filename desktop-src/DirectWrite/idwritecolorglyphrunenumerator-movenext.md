---
title: Идвритеколорглифруненумератор метод MoveNext
description: Переход к следующему глифу выполняется в перечислителе.
ms.assetid: E6336C0E-F880-485C-9111-A102298257C1
keywords:
- Прямая запись метода MoveNext
- Метод MoveNext Direct Write, интерфейс Идвритеколорглифруненумератор
- Прямая запись интерфейса Идвритеколорглифруненумератор, метод MoveNext
topic_type:
- apiref
api_name:
- IDWriteColorGlyphRunEnumerator.MoveNext
api_location:
- dwrite.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 15c9963916c07f1df8cf3cfedb49b9e3fd66d0df
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127470405"
---
# <a name="idwritecolorglyphrunenumeratormovenext-method"></a>Метод Идвритеколорглифруненумератор:: MoveNext

Переход к следующему глифу выполняется в перечислителе.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT MoveNext(
  [out] BOOL *haveRun
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*хаверун* \[ заполняет\]
</dt> <dd>

Тип: **bool \*** .

Возвращает **значение true** , если выполняется следующий запуск глифа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ приложения UWP для классических приложений \|\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Server 2012 Приложения универсального \[ приложения UWP для настольных приложений \|\]<br/>                          |
| Минимальный поддерживаемый телефон<br/>  | Windows Phone 8,1 \[ Windows Phone Silverlight 8,1 и среда выполнения Windows приложения\]<br/> |
| Библиотека<br/>                  | <dl> <dt>Дврите. lib</dt> </dl>   |
| DLL<br/>                      | <dl> <dt>Dwrite.dll</dt> </dl>   |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**идвритеколорглифруненумератор**](idwritecolorglyphrunenumerator.md)
</dt> </dl>

 

 





