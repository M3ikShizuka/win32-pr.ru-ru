---
description: Используйте эту заметку для определения содержимого внешнего файла в качестве значения инициализации для параметра effect.
ms.assetid: 3da1f951-cb8b-49ce-aba2-0badb3178093
title: Аннотация инициализации параметра
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c564b5b5e273b320fdc5de6148ef5ba5dd9f1b78
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126966573"
---
# <a name="parameter-initialization-annotation"></a>Аннотация инициализации параметра

Используйте эту заметку для определения содержимого внешнего файла в качестве значения инициализации для параметра effect. Пример:


```
string SasResourceAddress = "Value";
```



где value — это текстовая строка ASCII, которая может содержать абсолютный или относительный путь. Относительный путь относится к каталогу, содержащему файл эффектов.

Например:


```
texture2D DetailTexture
<
    string SasResourceAddress = "noise.dds";
>;
```



Значение по умолчанию — пустая строка.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Справочник по стандарту DirectX для заметок и семантик](dx9-graphics-reference-effects-dxsas.md)
</dt> </dl>

 

 



