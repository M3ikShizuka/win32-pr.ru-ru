---
title: Инверсия исходного регистра
description: Выполняет вычисление (1 значение) для каждого канала указанного регистра.
ms.assetid: 387e409f-d76d-4d70-be0f-fb563f542482
ms.topic: article
ms.date: 05/31/2018
topic_type:
- kbArticle
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: ce65960474816a91eb64ece7b754b97090903d46
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127264008"
---
# <a name="source-register-invert"></a>Инверсия исходного регистра

Выполняет вычисление (1 значение) для каждого канала указанного регистра.

## <a name="syntax"></a>Синтаксис


```
1 - register
```



## <a name="registers"></a>Регистры

Исходный регистр. Дополнительные сведения о типах регистров см. в описании [ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ регистров PS 1 1 PS 1 2](dx9-graphics-reference-asm-ps-registers-ps-1-x.md)PS 1 3 PS 1 4.

## <a name="remarks"></a>Remarks

Содержимое регистра не изменяется. Модификатор применяется только к данным, считанным из регистра. Операция инвертирования применяется ко всем четырем цветовым каналам (RGBA).

Этот модификатор можно использовать только с арифметическими инструкциями. Кроме того, этот модификатор нельзя сочетать с другой [маской записи регистра назначения](dx9-graphics-reference-asm-ps-registers-modifiers-write-mask.md).

## <a name="example"></a>Пример

В этом примере используется инверсия для создания дополнения для Register R1.


```
mul r0, r0, 1-r1;
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Модификаторы исходных регистров исходного шейдера пикселей](dx9-graphics-reference-asm-ps-registers-modifiers-source.md)
</dt> </dl>

 

 




