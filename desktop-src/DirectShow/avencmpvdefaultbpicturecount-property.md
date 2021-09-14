---
description: Указывает число последовательных кадров B между кадрами I и P по умолчанию.
ms.assetid: d41ed713-0159-4325-bc44-f4a3eea10aa2
title: Свойство Авенкмпвдефаултбпиктурекаунт (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d2026ddcb6a2b4ce813bd8ba2f6144f0c4a32344
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127148385"
---
# <a name="avencmpvdefaultbpicturecount-property"></a>Авенкмпвдефаултбпиктурекаунт, свойство

Указывает число последовательных кадров B между кадрами I и P по умолчанию.

Это свойство доступно для чтения и записи.

## <a name="data-type"></a>Тип данных

**UINT32** (**VT \_ UI4**)

## <a name="property-guid"></a>GUID свойства

**КОДЕКАПИ \_ авенкмпвдефаултбпиктурекаунт**

## <a name="property-value"></a>Значение свойства

Это свойство имеет линейный Диапазон значений. Чтобы получить поддерживаемый диапазон, вызовите метод [**икодекапи:: жетпараметерранже**](/windows/desktop/api/Strmif/nf-strmif-icodecapi-getparameterrange).

## <a name="remarks"></a>Remarks

до Windows 8 это свойство применяется к кодировщикам видео MPEG. начиная с Windows 8 это свойство используется кодировщиками видео MPEG, WMV и H. 264.

Если кодировщик поддерживает это свойство, его можно использовать для управления структурой групп рисунков (GOP).

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

 

 




