---
description: Отменяет регистрацию связанного поставщика.
ms.assetid: b5edc33d-dfd0-4350-b8cd-eaa30b726771
title: 'Метод Итипаутокомплетеклиент:: Унадвисепровидер (Типаутокомплете. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ITipAutocompleteClient.UnadviseProvider
api_type:
- COM
api_location:
- tiptsf.dll
ms.openlocfilehash: 1100ebb700ef2fb769a13f9b62aacf5c1d007e0d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127579442"
---
# <a name="itipautocompleteclientunadviseprovider-method"></a>Метод Итипаутокомплетеклиент:: Унадвисепровидер

Отменяет регистрацию связанного поставщика.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT UnadviseProvider(
  [in] HWND                   hWndField,
  [in] ITipAutocompleProvider *pIACProvider
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*хвндфиелд* \[ окне\]
</dt> <dd>

Описатель окна поля, предоставляющего функцию автозавершения.

</dd> <dt>

*пиакпровидер* \[ окне\]
</dt> <dd>

Указатель интерфейса на интерфейс поставщика автозавершения для отмены регистрации.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод может возвращать одно из этих значений.



| Код возврата                                                                            | Описание                               |
|----------------------------------------------------------------------------------------|-------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>   | Успешно.<br/>                       |
| <dl> <dt>**\_Ошибка E**</dt> </dl> | Произошла неизвестная ошибка.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                                   |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                                       |
| Заголовок<br/>                   | <dl> <dt>Типаутокомплете. h (также требуется Пенинпутпанел \_ i. c)</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Tiptsf.dll</dt> </dl>                                           |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Итипаутокомплетеклиент**](itipautocompleteclient.md)
</dt> <dt>

[Справочник по панели ввода текста](text-input-panel-reference.md)
</dt> </dl>

 

 




