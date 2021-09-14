---
title: Смещение исходного регистра
description: Вычтите 0,5 из всех компонентов.
ms.assetid: 6e1e96b0-e265-4b43-a9cb-8435e1fe891c
ms.topic: article
ms.date: 05/31/2018
topic_type:
- kbArticle
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 5c564dad0d4caf859ae00155dfd9619d90276cf1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127264011"
---
# <a name="source-register-bias"></a>Смещение исходного регистра

Вычтите 0,5 из всех компонентов.

## <a name="registers"></a>Регистры

Исходный регистр. Дополнительные сведения о типах регистров см. в описании [ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ регистров PS 1 1 PS 1 2](dx9-graphics-reference-asm-ps-registers-ps-1-x.md)PS 1 3 PS 1 4.

## <a name="remarks"></a>Remarks

Содержимое регистра не изменяется. Модификатор применяется только к данным, считанным из регистра. Этот сдвиг применяется ко всем четырем цветовым каналам (RGBA) следующим образом:


```
output = (input - 0.5)
```



Результатом является изменение данных, которые находятся в диапазоне от 0 до 1, в диапазоне от-0,5 до 0,5. Применение смещения к данным за пределами этого диапазона может привести к неопределенным результатам.

> [!Note]  
> Этот модификатор является взаимоисключающим с [инверсией в исходном регистре](dx9-graphics-reference-asm-ps-registers-modifiers-invert.md), поэтому он не может быть применен к тому же регистру.

 

Этот модификатор предназначен для использования с арифметическими инструкциями.

## <a name="example"></a>Пример

В этом примере выполняется та же операция, что и для D3DTOP \_ аддсигнед в DirectX 6,0 и 7,0 с несколькими синтаксисами текстуры.


```
add r0, r0, t0_bias; Shift down by 0.5.
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Модификаторы исходных регистров исходного шейдера пикселей](dx9-graphics-reference-asm-ps-registers-modifiers-source.md)
</dt> </dl>

 

 




