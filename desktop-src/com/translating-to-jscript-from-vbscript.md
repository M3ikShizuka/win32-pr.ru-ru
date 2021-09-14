---
title: перевод в JScript из VBScript
description: перевод в JScript из VBScript
ms.assetid: cdf04a01-8bc3-4f37-872b-3a0aae962f26
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a18c2ccb11ffa4f5f000d8cfc73f7db6f857cf6b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127253033"
---
# <a name="translating-to-jscript-from-vbscript"></a>перевод в JScript из VBScript

В VBScript **для**... **Каждый** цикл выполняет перечисление элементов коллекции. в JScript, **для**... **в** loop выполняет перечисление элементов объекта JScript или массива. чтобы перечислить коллекцию в JScript, используйте объект перечислителя.

в JScript существует несколько типов данных, таких как числа, строки, логические значения, объекты и атрибут null. В VBScript используется только один тип данных **Variant**, который может быть подтипа для представления строк, чисел, логических значений и т. д.

в JScript массивы можно развертывать динамически, задав новое значение для свойства length массива. В VBScript массивы не могут быть увеличены; они должны быть переизмерены с помощью оператора **ReDim** .

функции поддержки VBScript и JScript. Однако VBScript также поддерживает подпрограммы. Подпрограммы похожи на функции, но не возвращают значение.

JScript учитывает регистр. Язык VBScript не является.

JScript поддерживается как Internet Explorer, так и Netscape navigator. Netscape Navigator не поддерживает VBScript.

JScript предоставляет объект Error, который может использоваться для перехвата и обработки ошибок. Объект Error является аналогом объекта VBScript Err.

массивы JScript не являются массивами типа **VARIANT SAFEARRAY**. Если скрипт получает переменную **SAFEARRAY типа Variant** из COM-объекта или скрипта VBScript, он должен использовать объект VBArray для доступа к переменной **типа SafeArray** .

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Перевод в JScript](translating-to-jscript.md)
</dt> </dl>

 

 




