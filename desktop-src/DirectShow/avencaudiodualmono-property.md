---
description: Свойство Авенкаудиодуалмоно — указывает, кодируется ли двухканальный аудио-канал как стерео или два Mono.
ms.assetid: 37f25590-69c2-43bd-a5d4-2262457cb39d
title: Свойство Авенкаудиодуалмоно (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c7255177290ebbe15104d0264a821e9c17ecdf90b605fbaab435f6d39c577548
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120052824"
---
# <a name="avencaudiodualmono-property"></a>Авенкаудиодуалмоно, свойство

Указывает, кодируется ли двухканальный аудио-канал как стерео или два Mono.

Это свойство доступно для чтения и записи.

## <a name="data-type"></a>Тип данных

**UINT32** (**VT \_ UI4**)

## <a name="property-guid"></a>GUID свойства

**КОДЕКАПИ \_ авенкаудиодуалмоно**

## <a name="property-value"></a>Значение свойства

Значение этого свойства является членом перечисления [**еавенкаудиодуалмоно**](/windows/win32/api/codecapi/ne-codecapi-eavencaudiodualmono) .

## <a name="remarks"></a>Remarks

Это свойство не применяется к кодировщикам аудио в формате MPEG. Для звука MPEG используйте свойство [**авенкмпакодингмоде**](avencmpacodingmode-property.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional приложения \[ UWP для классических приложений \|\]<br/>                     |
| Минимальная версия сервера<br/> | \[приложения UWP для классических приложений Windows 2000 \|\]<br/>                           |
| Заголовок<br/>                   | <dl> <dt>Кодекапи. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Свойства кодека API](codec-api-properties.md)
</dt> <dt>

[**Интерфейс Икодекапи**](/windows/desktop/api/Strmif/nn-strmif-icodecapi)
</dt> </dl>

 

