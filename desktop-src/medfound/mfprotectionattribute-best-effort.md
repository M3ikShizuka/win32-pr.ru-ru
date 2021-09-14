---
description: Задайте в качестве атрибута для объекта Имфаутпутсчема.
ms.assetid: 0CCCAB27-DEB0-41D8-A70C-D6CCEFE0601F
title: Атрибут MFPROTECTIONATTRIBUTE_BEST_EFFORT (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: fd7d2f173b5bf85080e0de65866f84b3a317b7ac
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127346519"
---
# <a name="mfprotectionattribute_best_effort-attribute"></a>МФПРОТЕКТИОНАТТРИБУТЕный \_ атрибут с наилучшими \_ усилиями

Задайте в качестве атрибута для объекта [**имфаутпутсчема**](/windows/desktop/api/mfidl/nn-mfidl-imfoutputschema) . Если этот атрибут имеется, неудачная попытка применения защиты игнорируется. Если значение связанного атрибута равно **true**, следует применить схему защиты с атрибутом [мфпротектионаттрибуте \_ отработки отказа \_](mfprotectionattribute-fail-over.md) .

## <a name="data-type"></a>Тип данных

**Bool** , сохраненный как **UINT32**

## <a name="remarks"></a>Remarks

Если **значение — true**, принудительно Примените схему защиты с атрибутом [мфпротектионаттрибуте \_ \_ отработки отказа](mfprotectionattribute-fail-over.md) , если установить эту защиту не удается.

Задайте в качестве атрибута для объекта [**имфаутпутсчема**](/windows/desktop/api/mfidl/nn-mfidl-imfoutputschema) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ Только приложения UWP\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ Только приложения UWP\]<br/>                                   |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты типа мультимедиа](media-type-attributes.md)
</dt> </dl>

 

 




