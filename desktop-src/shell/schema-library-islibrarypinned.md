---
description: '&lt;элемент ислибрарипиннед &gt; указывает, закреплена ли эта библиотека на панели навигации в обозревателе Windows Explorer. Этот элемент является необязательным и не имеет дочерних элементов и атрибутов.'
title: Элемент Ислибрарипиннед (схема библиотеки)
ms.topic: article
ms.date: 05/31/2018
ms.assetid: AD8307E5-5676-4d43-8FEE-695F168F677D
api_name: ''
api_type: ''
api_location: ''
topic_type:
- kbArticle
ms.openlocfilehash: a535619fd38a0a557546f97f0a6ace64a065b61c
ms.sourcegitcommit: 61a4c522182aa1cacbf5669683d9570a3bf043b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122885640"
---
# <a name="islibrarypinned-element-library-schema"></a>Элемент Ислибрарипиннед (схема библиотеки)

&lt;элемент ислибрарипиннед &gt; указывает, закреплена ли эта библиотека на панели навигации в обозревателе Windows Explorer. Этот элемент является необязательным и не имеет дочерних элементов и атрибутов.

## <a name="syntax"></a>Синтаксис


```
<!-- isLibraryPinned -->
    <xs:element name="isLibraryPinned" type="xs:boolean" default="false" minOccurs="0"/>
```



## <a name="element-information"></a>Сведения об элементе



| Родительский элемент                                                               | Дочерние элементы |
|------------------------------------------------------------------------------|----------------|
| [Элемент Либраридескриптион (схема библиотеки)](schema-librarydescription.md) |                |



 

## <a name="remarks"></a>Комментарии

если значение — true, библиотека закреплена на панели навигации обозревателя Windows.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Элемент Либраридескриптион (схема библиотеки)](schema-librarydescription.md)
</dt> <dt>

[Элемент Сеарчконнектордескриптион (схема библиотеки)](schema-library-searchconnectordescription.md)
</dt> </dl>

 

 



