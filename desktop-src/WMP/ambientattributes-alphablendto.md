---
title: Амбиентаттрибутес. Алфаблендто
description: Метод Алфаблендто корректирует свойство Алфабленд за определенный период времени.
ms.assetid: 5cb259bd-3010-4086-be9d-65022be297b7
keywords:
- амбиентаттрибутес. алфаблендто проигрыватель Windows Media
topic_type:
- apiref
api_name:
- AmbientAttributes.alphaBlendTo
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 16b21e78de3510e2e4a58c7214995f7888f778c1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126890040"
---
# <a name="ambientattributesalphablendto"></a>Амбиентаттрибутес. Алфаблендто

Метод **алфаблендто** корректирует свойство **алфабленд** за определенный период времени.

``` syntax
        elementID.alphaBlendTo(newVal, alphaTime)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="newVal"></span><span id="newval"></span><span id="NEWVAL"></span>*неввал*
</dt> <dd>

**Число** (длинное), указывающее новое значение непрозрачности. Диапазон от 0 (без непрозрачности) до 255 (полная непрозрачность).

</dd> <dt>

<span id="alphaTime"></span><span id="alphatime"></span><span id="ALPHATIME"></span>*алфатиме*
</dt> <dd>

**Число** (**длинное**), указывающее время в миллисекундах, которое принимает элемент на изменение непрозрачности.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

Этот метод полезен для постепенного отображения или исчезновения элементов.

При использовании **алфаблендто** с **текстовым** элементом, для которого не указан **backgroundColor** , будет использоваться цвет фона черного цвета. Если цвет переднего плана также является черным (значением по умолчанию для *текста*).**foregroundColor**), текст может стать нечитаемым. Чтобы избежать этого, всегда указывайте атрибут **backgroundColor** или задайте для **foregroundColor** цвет, отличный от черного.

> [!Note]  
> этот атрибут не поддерживается в Windows 98.

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Атрибуты окружения**](ambient-attributes.md)
</dt> <dt>

[**Амбиентаттрибутес. Алфабленд**](ambientattributes-alphablend.md)
</dt> <dt>

[**TEXT, элемент**](text-element.md)
</dt> <dt>

[**TEXT. backgroundColor**](text-backgroundcolor.md)
</dt> <dt>

[**TEXT. foregroundColor**](text-foregroundcolor.md)
</dt> </dl>

 

 





