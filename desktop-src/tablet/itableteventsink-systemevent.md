---
description: Происходит при наличии системного события.
ms.assetid: 3d9e98f0-b11e-4a65-a544-9e1998a80d5f
title: 'Метод Итаблетевентсинк:: Системевент'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ITabletEventSink.SystemEvent
api_type:
- COM
api_location:
- wisptis.exe
- wisptis.exe.dll
ms.openlocfilehash: 71b5882fd9e19df43581e00cce55c2af5faa432b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460224"
---
# <a name="itableteventsinksystemevent-method"></a>Метод Итаблетевентсинк:: Системевент

Происходит при наличии системного события.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SystemEvent(
  [in] TABLET_CONTEXT_ID tcid,
  [in] CURSOR_ID         cid,
  [in] SYSTEM_EVENT      event,
  [in] SYSTEM_EVENT_DATA eventdata
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*тЦид* \[ окне\]
</dt> <dd>

Идентификатор планшета.

</dd> <dt>

*CID* \[ в\]
</dt> <dd>

Идентификатор пера.

</dd> <dt>

*событие* \[ окне\]
</dt> <dd>

Код системного события.

</dd> <dt>

*EVENTDATA* \[ окне\]
</dt> <dd>

Данные системных событий.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод может возвращать одно из этих значений.



| Код возврата                                                                            | Описание                               |
|----------------------------------------------------------------------------------------|-------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>   | Успешно.<br/>                       |
| <dl> <dt>**\_Ошибка E**</dt> </dl> | Произошла неизвестная ошибка.<br/> |



 

## <a name="remarks"></a>Remarks

Следующий список содержит допустимые значения для параметра события.

-   SE \_ ЭЛЕМЕНТА
-   SE \_ ДВОЙНОЕ \_ касание
-   SE \_ ПРАВОе \_ касание
-   SE \_ ПЕРЕМЕСТИТЬ
-   SE \_ Перетаскивание правой кнопкой мыши \_
-   SE \_ удерживайте клавишу \_ Ввод
-   SE \_ УДЕРЖИВАТЬ \_ оставить
-   SE \_ ввод с наведением \_
-   SE \_ выход при наведении \_
-   SE \_ Средний \_ щелчок
-   SE \_ РАЗДЕЛ
-   SE \_ \_Клавиша модификатора
-   SE \_ \_режим жестов
-   SE \_ НАБОРА

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                              |
| Библиотека<br/>                  | <dl> <dt>Wisptis.exe</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Итаблетевентсинк**](itableteventsink.md)
</dt> </dl>

 

 




