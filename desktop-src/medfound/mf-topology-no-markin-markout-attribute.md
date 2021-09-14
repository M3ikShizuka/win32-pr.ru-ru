---
description: Указывает, обрезает ли образцы в конвейере.
ms.assetid: 4ba66d18-3854-4994-9509-967303dc7d98
title: Атрибут MF_TOPOLOGY_NO_MARKIN_MARKOUT (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 03d7b0152798379406887619a3e691cc528a6993
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127346558"
---
# <a name="mf_topology_no_markin_markout-attribute"></a>\_Топология \_ MF \_ отсутствует \_ атрибут Маркин Mark

Указывает, обрезает ли образцы в конвейере.

## <a name="data-type"></a>Тип данных

**UINT32**

Рассматривать как логическое значение.

## <a name="remarks"></a>Remarks

По умолчанию конвейер обрезает образцы в соответствии с правильным временем представления. Усечение выполняется на узлах топологии с атрибутами [**MF \_ топоноде \_ Маркин \_ здесь**](mf-toponode-markin-here-attribute.md) и [**MF \_ топоноде \_ меток \_**](mf-toponode-markout-here-attribute.md) . Если **для топологии** **MF не задан атрибут \_ \_ \_ Маркин \_ Mark** , то конвейер не усекает выборки, а **MF \_ топоноде \_ Маркин \_ здесь** и **MF топоноде. \_ \_ \_ здесь** атрибуты игнорируются. Если атрибут не задан или имеет значение **false**, конвейер усекает выборки.

Приложение может задать для параметра **" \_ топология MF \_ No \_ Маркин \_ Mark** " **значение true** , если приложение получает сжатые образцы из конвейера и должно получить все ключевые кадры, которые в противном случае могут быть обрезаны.

Значение этого атрибута по умолчанию равно **false**.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: UINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32)
</dt> <dt>

[**Имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32)
</dt> <dt>

[**MF \_ топоноде \_ Маркин \_**](mf-toponode-markin-here-attribute.md)
</dt> <dt>

[**Разметка MF \_ топоноде \_ \_**](mf-toponode-markout-here-attribute.md)
</dt> <dt>

[Атрибуты топологии](topology-attributes.md)
</dt> </dl>

 

 




