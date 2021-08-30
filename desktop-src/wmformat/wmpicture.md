---
title: WM/Picture
description: Атрибут WM/Picture содержит изображение, связанное с содержимым.
ms.assetid: ec82dfdf-7755-4758-9771-096aac114f78
keywords:
- Формат мультимедиа Windows WM/Picture
topic_type:
- apiref
api_name:
- WM/Picture
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8c0648cc82faae7a0bab9614761caef98c316fd73b5eb90550d14754386282f7
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120109934"
---
# <a name="wmpicture"></a>WM/Picture

Атрибут **WM/Picture** содержит изображение, связанное с содержимым.

## <a name="global-constant"></a>Глобальная константа

g \_ всзвмпиктуре

## <a name="data-type"></a>Тип данных

[**WM \_ Рисунок**](/previous-versions/windows/desktop/api/wmsdkidl/ns-wmsdkidl-wm_picture) (**\_ \_ двоичный тип ВМТ**)

## <a name="remarks"></a>Remarks

Этот атрибут совместим с кадром ID3, APIC. Спецификация ID3 для кадра APIC подразумевает, что, хотя может существовать любое количество кадров APIC, связанных с файлом, только один из них может иметь тип 1, а только один может иметь тип 2. В спецификации также указывается, что описание изображения не может содержать более 64 символов, но может быть пустым.

атрибуты WM/Picture, добавленные с помощью объектов пакета SDK для Windows Media Format, не проверяются автоматически в соответствии со спецификациями ID3. Необходимо добавить код в приложение для выполнения проверок, если требуется обеспечить полную совместимость с ID3.

## <a name="see-also"></a>См. также

<dl> <dt>

[**Список атрибутов**](attribute-list.md)
</dt> <dt>

[**\_изображение WM**](/previous-versions/windows/desktop/api/wmsdkidl/ns-wmsdkidl-wm_picture)
</dt> </dl>

 

 




