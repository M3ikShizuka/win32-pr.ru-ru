---
description: Метод Копивалуесфромпропертисторе копирует содержимое объекта Ипропертисторе в коллекцию.
ms.assetid: 887c9569-ff76-41cf-8782-62c59c04e831
title: 'Метод Ипортабледевицевалуес:: Копивалуесфромпропертисторе (Портабледевицетипес. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IPortableDeviceValues.CopyValuesFromPropertyStore
api_type:
- COM
api_location:
- PortableDeviceGUIDs.lib
- PortableDeviceGUIDs.dll
ms.openlocfilehash: 0944edff81a62652851bc2c18b58f47f5d33d09ad7da6ba5a2eda95919c54dd2
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118963713"
---
# <a name="iportabledevicevaluescopyvaluesfrompropertystore-method"></a>Метод Ипортабледевицевалуес:: Копивалуесфромпропертисторе

Метод **копивалуесфромпропертисторе** копирует содержимое объекта **ипропертисторе** в коллекцию.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT CopyValuesFromPropertyStore(
  [in] IPropertyStore *pStore
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pStore* \[ окне\]
</dt> <dd>

Указатель на **ипропертисторе** , который необходимо скопировать в коллекцию.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает **значение HRESULT**. Допустимые значения включают, но не ограничиваются, значения, приведенные в следующей таблице.



| Код возврата                                                                          | Описание                      |
|--------------------------------------------------------------------------------------|----------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl> | Метод выполнен успешно.<br/> |



 

## <a name="remarks"></a>Remarks

Этот метод автоматически преобразует все значения **VT \_ BSTR** в значения **VT \_ LPWSTR** .

Многие внешние приложения или компоненты, взаимодействующие с приложением, например некоторые приложения оболочки, используют интерфейс **ипропертисторе** . Этот метод обеспечивает быстрый и простой способ обмена данными с этими программами.

этот метод поддерживается в Windows Vista и более поздних версиях Windows.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Портабледевицетипес. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>Портабледевицегуидс. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ипортабледевицевалуес**](iportabledevicevalues.md)
</dt> <dt>

[**Ипортабледевицевалуес:: Копивалуестопропертисторе**](iportabledevicevalues-copyvaluestopropertystore.md)
</dt> </dl>

 

 




