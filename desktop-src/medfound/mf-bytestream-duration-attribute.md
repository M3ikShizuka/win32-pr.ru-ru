---
description: Задает длительность потока байтов в единицах 100-наносекундных.
ms.assetid: afa4930c-544b-4d66-94fe-9795bb526e0a
title: Атрибут MF_BYTESTREAM_DURATION (Мфобжектс. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: df264416b8a805e6d239cfcc457f4a6db2a8e4dc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462187"
---
# <a name="mf_bytestream_duration-attribute"></a>\_ \_ Атрибут длительности BYTESTREAM MF

Задает длительность потока байтов в единицах 100-наносекундных.

## <a name="data-type"></a>Тип данных

**UINT64**

Рассматривать как значение **лонглонг** .

## <a name="remarks"></a>Remarks

Этот атрибут является необязательным. Если объект, создающий байтовый поток, может определить длительность, он может установить этот атрибут. (Например, в сетевом потоке длительность может быть частью описания сеанса.)

Чтобы получить значение атрибута, вызовите метод **QueryInterface** в байтовом потоке, чтобы получить указатель на интерфейс [**имфаттрибутес**](/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes) .

Этот атрибут имеет значение со знаком, хотя оно хранится в виде **UINT64**.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Приложения UWP для классических приложений Vista \|\]<br/>                                                    |
| Минимальная версия сервера<br/> | Windows \[Приложения UWP для классических приложений сервера 2008 \|\]<br/>                                              |
| Заголовок<br/>                   | <dl> <dt>Мфобжектс. h (включение Мфидл. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты потока байтов](byte-stream-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: UINT64**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint64)
</dt> <dt>

[**Имфаттрибутес:: SetUINT64**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint64)
</dt> <dt>

[**имфбитестреам**](/windows/desktop/api/mfobjects/nn-mfobjects-imfbytestream)
</dt> </dl>

 

 




