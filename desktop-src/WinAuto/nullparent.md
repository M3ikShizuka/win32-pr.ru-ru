---
title: нуллпарент
description: нуллпарент
ms.assetid: F9563D73-66EF-4C66-8783-B034AA7A212E
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f265f66eb4d0b0985d9f3979fc7ff4b9bb1812df1617cdaa4f6f50d7b357e067
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119998154"
---
# <a name="nullparent"></a>нуллпарент

## <a name="text"></a>Текст

Родительский элемент Elements имеет значение NULL

## <a name="type"></a>Тип

Error

## <a name="description"></a>Описание

Значение NULL возвращается при вызове [**Get \_ аккпарент**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accparent) для элемента. Метод **Get \_ аккпарент** должен возвращать значение NULL только при вызове в корневом элементе целевого объекта проверки.

Эта проблема может вызвать проблемы с навигацией для автоматизированных средств, так как обходные элементы могут быть неустойчивыми и непредсказуемыми.

## <a name="possible-causes"></a>Возможные причины

Неправильная или недопустимая реализация MSAA.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**IAccessible:: Аккнавигате**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-accnavigate)
</dt> <dt>

[**IAccessible:: Get \_ аккпарент**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accparent)
</dt> </dl>

 

 




