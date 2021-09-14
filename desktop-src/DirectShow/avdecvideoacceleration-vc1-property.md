---
description: Включает или отключает аппаратное ускорение для декодирования видео VC-1.
ms.assetid: eee85330-098e-4f21-81b7-a493abbd599b
title: Свойство AVDecVideoAcceleration_VC1 (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1fcdbe265f5a65212a2846b724f570b024ea0ab8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127162111"
---
# <a name="avdecvideoacceleration_vc1-property"></a>Авдеквидеоакцелератион \_ VC1, свойство

Включает или отключает аппаратное ускорение для декодирования видео VC-1.

Это свойство доступно для чтения и записи.

## <a name="data-type"></a>Тип данных

**UINT32** (**VT \_ UI4**)

## <a name="property-guid"></a>GUID свойства

**КОДЕКАПИ \_ авдеквидеоакцелератион \_ VC1**

## <a name="remarks"></a>Комментарии

Если значение равно нулю, декодер не использует ускорение видео DirectX (ДКСВА) для декодирования видео VC-1. для DirectShow фильтров установите это свойство перед подключением выходного пин-кода декодера.

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

 

 




