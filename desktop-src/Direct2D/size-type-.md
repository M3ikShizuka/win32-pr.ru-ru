---
title: Функция типа size (D2d1helper. h)
description: Создает структуру размера, в которой хранятся значения ширины и высоты, используя указанный тип данных.
ms.assetid: 9f7e37a3-440e-40c0-a527-9fcbd207dce8
keywords:
- Тип размера функция Direct2D
topic_type:
- apiref
api_name:
- Size Type Function
api_location:
- D2d1.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 39d689d5f5c729e13385fc0d6d5b31baf96b141b
ms.sourcegitcommit: 61a4c522182aa1cacbf5669683d9570a3bf043b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122886989"
---
# <a name="sizelttypegt-function"></a>Тип size, &lt; &gt; функция

Создает структуру размера, в которой хранятся значения ширины и высоты, используя указанный тип данных.

``` syntax
template<typename Type>
typename TypeTraits<Type>::Size Size(
  Type width,
  Type height
);
```

## <a name="template-parameters"></a>Параметры шаблона



| Параметр | Описание                                                                                         |
|-----------|-----------------------------------------------------------------------------------------------------|
| Тип      | Тип данных, используемый для хранения ширины и высоты размера. Возможными значениями являются FLOAT и UINT32. |



 

## <a name="parameters"></a>Параметры



| Параметр | Описание        |
|-----------|--------------------|
| width     | Ширина размера.  |
| рост    | Высота размера. |



 

## <a name="return-value"></a>Возвращаемое значение

Размер, который содержит указанные ширину и высоту.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 7, Windows Vista с пакетом обновления 2 (SP2) и обновлением платформы для приложений для \[ классических приложений Windows Vista \|\]<br/>                          |
| Минимальная версия сервера<br/> | Windows сервер 2008 R2, Windows Server 2008 с пакетом обновления 2 (SP2) и обновлением платформы для Windows Server 2008 приложения \[ UWP для классических приложений \|\]<br/> |
| Минимальный поддерживаемый телефон<br/>  | Windows Phone 8,1 \[ Windows Phone Silverlight 8,1 и среда выполнения Windows приложения\]<br/>                                                  |
| Заголовок<br/>                   | <dl> <dt>D2d1helper. h</dt> </dl>                                                  |
| Библиотека<br/>                  | <dl> <dt>D2d1. lib</dt> </dl>                                                      |
| DLL<br/>                      | <dl> <dt>D2d1.dll</dt> </dl>                                                      |



 

 





