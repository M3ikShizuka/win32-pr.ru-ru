---
title: Иконфигасфвритер Конфигурефилтерусингпрофилегуид, метод
description: Метод Конфигурефилтерусингпрофилегуид настраивает фильтр для записи файла ASF на основе указанного заранее заданного профиля. (Не рекомендуется.).
ms.assetid: 94161ee7-1b74-47af-9d77-568abe6237c3
keywords:
- Формат Windows Media, Конфигурефилтерусингпрофилегуид метод
- Конфигурефилтерусингпрофилегуид метод Windows Media Format, интерфейс Иконфигасфвритер
- Интерфейс Иконфигасфвритер Windows Media Format, метод Конфигурефилтерусингпрофилегуид
topic_type:
- apiref
api_name:
- IConfigAsfWriter.ConfigureFilterUsingProfileGuid
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: a1521738af4411baa2c11f3d20722e09e2d22a83
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458740"
---
# <a name="iconfigasfwriterconfigurefilterusingprofileguid-method"></a>Метод Иконфигасфвритер:: Конфигурефилтерусингпрофилегуид

Метод **конфигурефилтерусингпрофилегуид** настраивает фильтр для записи файла ASF на основе указанного заранее заданного профиля. (Не рекомендуется.)

## <a name="syntax"></a>Синтаксис


```C++
HRESULT ConfigureFilterUsingProfileGuid(
  [in] REFGUID guidProfile
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*гуидпрофиле* \[ окне\]
</dt> <dd>

**GUID** , определяющий профиль, как определено в файле заголовка пакета SDK для Windows Media Format вмсиспрф. h.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из следующих значений **HRESULT** .



| Код возврата                                                                                         | Описание                             |
|-----------------------------------------------------------------------------------------------------|-----------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>                | Метод выполнен успешно.<br/>        |
| <dl> <dt>**\_Ошибка E**</dt> </dl>              | Недопустимый профиль.<br/>    |
| <dl> <dt>**VFW \_ E — \_ неправильное \_ состояние**</dt> </dl> | Граф фильтра остановлен.<br/> |



 

## <a name="remarks"></a>Remarks

начиная с пакета SDK серии для Windows Media Format 9, новые системные профили не определены. С этим методом можно использовать только идентификаторы GUID системного профиля версии 8 (или более ранней).

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Иконфигасфвритер**](/previous-versions/windows/desktop/legacy/dd743205(v=vs.85))
</dt> </dl>

 

