---
title: Атрибут Аверажелевел
description: Атрибут Аверажелевел представляет собой 16-битное значение амплитуды, указывающее средний уровень громкости.
ms.assetid: 04ff19f1-a9a5-4e47-86a6-50c6f08b0d7d
keywords:
- проигрыватель Windows Media атрибута аверажелевел
topic_type:
- apiref
api_name:
- AverageLevel
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 594612f3675d818f94270b1952d2a9ca7bed15d7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126889824"
---
# <a name="averagelevel-attribute"></a>Атрибут Аверажелевел

Атрибут **аверажелевел** представляет собой 16-битное значение амплитуды, указывающее средний уровень громкости.

## <a name="applies-to"></a>Применяется к

-   [Звуковые элементы](audio-item-attributes.md)
-   [часто используемые Windows файлы мультимедиа](commonly-used-windows-media-file-attributes.md)

## <a name="remarks"></a>Комментарии

Этот атрибут хранится как в библиотеке, так и в файле цифрового мультимедиа.

проигрыватель Windows Media задает это значение в одном из следующих экземпляров:

-   После копирования файла на скопированный файл.
-   После воспроизведения файла (при включенном улучшении автоматического выравнивания громкости).

константа пакета SDK Windows Media Format для этого атрибута — g \_ всзаверажелевел.

Чтобы определить, можно ли изменить значение этого атрибута, используйте метод [Media. исреадонлитем](media-isreadonlyitem.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Ссылка на атрибут**](attribute-reference.md)
</dt> </dl>

 

 





