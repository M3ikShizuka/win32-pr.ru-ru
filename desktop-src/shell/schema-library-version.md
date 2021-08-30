---
description: '&lt;Элемент Version &gt; указывает версию содержимого этой библиотеки. Этот элемент не имеет атрибутов и не содержит дочерних элементов.'
ms.assetid: 77FD5EF6-6B6F-48e1-973F-AC069F729613
title: Элемент Version (схема библиотеки)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ce1aeac399b5fa71b4a1ca57b63d8ecb95ede57f
ms.sourcegitcommit: 61a4c522182aa1cacbf5669683d9570a3bf043b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122885460"
---
# <a name="version-element-library-schema"></a>Элемент Version (схема библиотеки)

&lt;Элемент Version &gt; указывает версию содержимого этой библиотеки. Этот элемент не имеет атрибутов и не содержит дочерних элементов.

## <a name="syntax"></a>Синтаксис

``` syntax
<!-- version -->
<xs:element name="version" type="xs:int" minOccurs="0"/>
```

## <a name="element-information"></a>Сведения об элементе



| Родительский элемент                                                               | Дочерние элементы |
|------------------------------------------------------------------------------|----------------|
| [Элемент Либраридескриптион (схема библиотеки)](schema-librarydescription.md) | None           |



 

## <a name="remarks"></a>Remarks

Версия содержимого библиотеки отличается от версии в формате файла библиотеки ( \* . Library-MS). Версия формата файла библиотеки указывается в [пространстве имен](library-schema-entry.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Схема описания библиотеки](library-schema-entry.md)
</dt> <dt>

[Схема описания соединителя поиска](../search/search-sconn-desc-schema-entry.md)
</dt> </dl>

 

 
