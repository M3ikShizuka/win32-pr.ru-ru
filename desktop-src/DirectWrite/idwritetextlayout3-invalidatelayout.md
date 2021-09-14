---
title: IDWriteTextLayout3 Инвалидателайаут, метод
description: Делает макет недействительным, принудительно перемера макета перед вызовом метрик или функций рисования. Это полезно в том случае, если изменяется расположение шрифта, а макет должен быть перерисован или если размер, реализуемый клиентом, Идвритеинлинеобжект изменения.
ms.assetid: 65b42ee1-5b67-1f6d-0e4b-ee60b192e7b7
keywords:
- Непосредственная запись метода Инвалидателайаут
- Прямая запись метода Инвалидателайаут, интерфейс IDWriteTextLayout3
- Прямая запись интерфейса IDWriteTextLayout3, метод Инвалидателайаут
topic_type:
- apiref
api_name:
- IDWriteTextLayout3.InvalidateLayout
api_location:
- dwrite.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b5df97d4590f62f586a570d52428b6560a7d88df
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127144846"
---
# <a name="idwritetextlayout3invalidatelayout-method"></a>Метод IDWriteTextLayout3:: Инвалидателайаут

Делает макет недействительным, принудительно перемера макета перед вызовом метрик или функций рисования. Это полезно в том случае, если изменяется расположение шрифта, а макет должен быть перерисован или если размер, реализуемый клиентом, Идвритеинлинеобжект изменения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT InvalidateLayout();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                                 |
| Минимальный поддерживаемый телефон<br/>  | Windows Phone 8,1 \[ Windows Phone Silverlight 8,1 и среда выполнения Windows приложения\]<br/> |
| Библиотека<br/>                  | <dl> <dt>Дврите. lib</dt> </dl>   |
| DLL<br/>                      | <dl> <dt>Dwrite.dll</dt> </dl>   |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**IDWriteTextLayout3**](idwritetextlayout3.md)
</dt> </dl>

 

 





