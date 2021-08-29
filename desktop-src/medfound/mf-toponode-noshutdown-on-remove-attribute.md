---
description: Указывает, как сеанс мультимедиа завершает работу объекта в топологии.
ms.assetid: 53b4faba-860f-4d6c-a145-09ea4ae63b8b
title: Атрибут MF_TOPONODE_NOSHUTDOWN_ON_REMOVE (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3bb7db9a883db80cc6154c72d2c4218b7815456b
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122477100"
---
# <a name="mf_toponode_noshutdown_on_remove-attribute"></a>MF \_ ТОПОНОДЕ \_ отключение \_ при \_ удалении атрибута

Указывает, как сеанс мультимедиа завершает работу объекта в топологии.

## <a name="data-type"></a>Тип данных

**UINT32**

Рассматривать как логическое значение.

## <a name="remarks"></a>Комментарии

Этот атрибут применяется к следующим типам узлов топологии:

-   Выходные узлы
-   Любой узел преобразования, содержащий *асинхронное* преобразование Media Foundation (MFT).

Атрибут может иметь следующие значения:




| Значение | Описание | 
|-------|-------------|
| <strong>TRUE</strong> | Когда сеанс мультимедиа переключается на новую топологию или очищает текущую топологию, он не завершает работу объекта, принадлежащего этому узлу топологии. | 
| <strong>FALSE</strong> | Когда сеанс мультимедиа переключается на новую топологию или очищает текущую топологию, он завершает работу объекта node следующим образом:<ul><li>Выходные узлы. сеанс вызывает <a href="/windows/desktop/api/mfidl/nf-mfidl-imfmediasink-shutdown"><strong>имфмедиасинк:: Shutdown</strong></a> в приемнике носителя.</li><li>Узлы преобразования. сеанс вызывает <a href="/windows/desktop/api/mfidl/nf-mfidl-imfshutdown-shutdown"><strong>имфшутдовн:: Shutdown</strong></a> в MFT.</li></ul> | 




 

Значение по умолчанию — **true**.

Если приложение помещает в очередь несколько топологий, рекомендуется присвоить этому атрибуту значение **false**. В противном случае объекты в топологии могут быть неправильно закрыты.

Этот атрибут не применяется, когда приложение завершает сеанс мультимедиа путем вызова [**имфмедиасессион:: Shutdown**](/windows/desktop/api/mfidl/nf-mfidl-imfmediasession-shutdown). Когда сеанс мультимедиа завершает работу, он всегда завершает работу приемников носителей и асинхронных МФТС в текущей топологии.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Асинхронный МФТС](asynchronous-mfts.md)
</dt> <dt>

[Атрибуты узла топологии](topology-node-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: UINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32)
</dt> <dt>

[**Имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32)
</dt> <dt>

[**имфтопологиноде**](/windows/desktop/api/mfidl/nn-mfidl-imftopologynode)
</dt> </dl>

 

 




