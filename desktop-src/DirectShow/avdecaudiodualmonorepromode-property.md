---
description: Указывает, как декодер воспроизводит два моно аудио.
ms.assetid: 3ef1f52c-13b2-4d9f-99fe-3317846be8a0
title: Свойство Авдекаудиодуалмонорепромоде (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a71ebe7e003b2dc4b6eebc30901525ffb918a9a9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127162155"
---
# <a name="avdecaudiodualmonorepromode-property"></a>Авдекаудиодуалмонорепромоде, свойство

Указывает, как декодер воспроизводит два моно аудио.

Это свойство доступно для чтения и записи.

## <a name="data-type"></a>Тип данных

**UINT32** (**VT \_ UI4**)

## <a name="property-guid"></a>GUID свойства

**КОДЕКАПИ \_ авдекаудиодуалмонорепромоде**

## <a name="property-value"></a>Значение свойства

Значение этого свойства является членом перечисления [**еавдекаудиодуалмонорепромоде**](/windows/desktop/api/codecapi/ne-codecapi-eavdecaudiodualmonorepromode) .

## <a name="remarks"></a>Комментарии

Эти свойства применяются только в том случае, если входной поток битов декодера содержит два моно аудио. Чтобы проверить это условие, получите значение свойства [авдекаудиодуалмоно](avdecaudiodualmono-property.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional приложения \[ UWP для классических приложений \|\]<br/>                     |
| Минимальная версия сервера<br/> | \[приложения UWP для классических приложений Windows 2000 \|\]<br/>                           |
| Заголовок<br/>                   | <dl> <dt>Кодекапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства кодека API](codec-api-properties.md)
</dt> <dt>

[**Интерфейс Икодекапи**](/windows/desktop/api/Strmif/nn-strmif-icodecapi)
</dt> </dl>

 

 




