---
description: Свойство Авенкаудиодуалмоно — указывает, кодируется ли двухканальный аудио-канал как стерео или два Mono.
ms.assetid: 37f25590-69c2-43bd-a5d4-2262457cb39d
title: Свойство Авенкаудиодуалмоно (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b58cbd901079d8f4dede1efae140791ae99c7fed
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127162068"
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

## <a name="remarks"></a>Комментарии

Это свойство не применяется к кодировщикам аудио в формате MPEG. Для звука MPEG используйте свойство [**авенкмпакодингмоде**](avencmpacodingmode-property.md) .

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

 

