---
title: Отрицательный Регистр исходного регистра
description: Выполняет отрицание (y-x) для всех компонентов регистрации.
ms.assetid: fe11f7a7-81be-4237-8194-15704f6fe43c
ms.topic: article
ms.date: 05/31/2018
topic_type:
- kbArticle
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 2f6082523926d70e670e0b792c6e7e8f41c7c1a0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127345851"
---
# <a name="source-register-negate"></a>Отрицательный Регистр исходного регистра

Выполняет отрицание (y =-x) для всех компонентов регистрации.

## <a name="syntax"></a>Синтаксис


```
- register
```



## <a name="registers"></a>Регистры

Исходный регистр. Дополнительные сведения о типах регистров см. в описании [ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ \_ регистров PS 1 1 PS 1 2](dx9-graphics-reference-asm-ps-registers-ps-1-x.md)PS 1 3 PS 1 4.

## <a name="remarks"></a>Remarks

Содержимое регистра не изменяется. Модификатор применяется только к данным, считанным из регистра. Операция отрицания применяется ко всем четырем цветовым каналам (RGBA).

Эта операция выполняется после любого другого модификатора, присутствующего в том же аргументе.

Этот модификатор является взаимоисключающим с [инверсией исходного регистра](dx9-graphics-reference-asm-ps-registers-modifiers-invert.md) , поэтому он не может быть применен к тому же регистру.

Этот модификатор предназначен для использования только с арифметическими инструкциями.

## <a name="example"></a>Пример

В следующем примере показано, как использовать этот модификатор.


```
mul r0, r0, -v1;
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Модификаторы исходных регистров исходного шейдера пикселей](dx9-graphics-reference-asm-ps-registers-modifiers-source.md)
</dt> </dl>

 

 




