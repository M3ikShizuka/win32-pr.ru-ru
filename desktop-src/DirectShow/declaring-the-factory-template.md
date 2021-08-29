---
description: Объявление шаблона фабрики
ms.assetid: 3060c167-ea23-4061-b32a-16e750f55e6f
title: Объявление шаблона фабрики
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ab71a925df01eee1f6e8c4365de4f00afd32b3449aa6ee07bc949e225713c2cf
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118953193"
---
# <a name="declaring-the-factory-template"></a>Объявление шаблона фабрики

Следующим шагом является объявление шаблона фабрики для фильтра. Шаблон фабрики — это класс C++, который содержит сведения для фабрики класса. В библиотеке DLL объявите глобальный массив объектов [**кфакторитемплате**](cfactorytemplate.md) , по одному для каждого фильтра или COM-компонента в библиотеке DLL. Массив должен называться *g \_ Templates*. дополнительные сведения о шаблонах фабрики см. [в разделе создание библиотеки DLL фильтра DirectShow](how-to-create-a-dll.md).

Элемент **\_ \_ фильтра m памовиесетуп** шаблона фабрики — это указатель на структуру [**\_ фильтра амовиесетуп**](amoviesetup-filter.md) , описанную ранее. В следующем примере показан шаблон фабрики с использованием структуры, заданной в предыдущем примере.


```C++
CFactoryTemplate g_Templates[] = {
    {
        g_wszName,                      // Name.
        &CLSID_SomeFilter,              // CLSID.
        CSomeFilter::CreateInstance,    // Creation function.
        NULL,
        &sudFilterReg                   // Pointer to filter information.
    }
};
int g_cTemplates = sizeof(g_Templates) / sizeof(g_Templates[0]);
```



Если вы не объявили какие бы то ни было сведения о фильтре, **m \_ памовесетуп \_ Filter** может иметь **значение NULL**.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[как зарегистрировать фильтры DirectShow](how-to-register-directshow-filters.md)
</dt> </dl>

 

 



