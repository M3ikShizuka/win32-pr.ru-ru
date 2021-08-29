---
title: аккнамеконтаинсинвалидстринг
description: аккнамеконтаинсинвалидстринг
ms.assetid: 392E4D10-4A8E-4118-B0E7-F74571812043
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 681f9829f3675c469801e8f40325e83865e625b5f3496e865d1ec383c033b7f3
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119955984"
---
# <a name="accnamecontainsinvalidstring"></a>аккнамеконтаинсинвалидстринг

## <a name="text"></a>Текст

Аккнаме не должно содержать строку {0}

## <a name="type"></a>Тип

Error

## <a name="description"></a>Описание

Имя элемента содержит недопустимые символы (эти символы заменяются на Аккчеккер). Например, метод [**Get \_ аккнаме**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accname) , используемый для получения имени MSAA элемента, возвращает строку, содержащую символы табуляции, новой строки или амперсанда.

Эта проблема вызывает проблемы для тех, кто полагается на средство чтения с экрана и клавиатуру для навигации, так как элемент может иметь непонятное имя, не являющееся интуитивно понятным.

## <a name="possible-causes"></a>Возможные причины

Элемент или его родитель имеет неправильно назначенное имя или подпись.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**IAccessible:: Get \_ аккнаме**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accname)
</dt> <dt>

[Свойство Name](name-property.md)
</dt> </dl>

 

 




