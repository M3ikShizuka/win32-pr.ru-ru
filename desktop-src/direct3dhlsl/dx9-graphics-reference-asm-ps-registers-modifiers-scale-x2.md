---
title: Масштаб исходного регистра x 2
description: Умножьте значение на два, прежде чем использовать его в инструкции.
ms.assetid: a02c9572-e03d-410b-8b65-7ea1a0bfaa0f
ms.topic: article
ms.date: 05/31/2018
topic_type:
- kbArticle
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: fc07605d0b570ce9647a8091d9eef7f7a6ad4ecaaeee96ce2d04aaaa3d8bcdd4
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120024174"
---
# <a name="source-register-scale-x-2"></a>Масштаб исходного регистра x 2

Умножьте значение на два, прежде чем использовать его в инструкции.

## <a name="syntax"></a>Синтаксис


```
register_x2
```



## <a name="register"></a>Зарегистрировать

Исходный регистр. Дополнительные сведения о типах регистров см. в описании [ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ регистров PS 1 1 PS 1 2](dx9-graphics-reference-asm-ps-registers-ps-1-x.md)PS 1 3 PS 1 4.

## <a name="remarks"></a>Remarks

Содержимое регистра не изменяется. Модификатор применяется только к данным, считанным из регистра.

Этот модификатор является взаимоисключающим с [инверсией в исходном регистре](dx9-graphics-reference-asm-ps-registers-modifiers-invert.md), поэтому он не может быть применен к тому же регистру.

Этот модификатор доступен только для арифметических инструкций в версии 1 \_ 4.

## <a name="example"></a>Пример

В этом примере показана текстура, преобразование данных в диапазон от-1 до + 1 и вычисление произведения точки.


```
mul r0, r0, r1_x2;
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Модификаторы исходных регистров исходного шейдера пикселей](dx9-graphics-reference-asm-ps-registers-modifiers-source.md)
</dt> </dl>

 

 




