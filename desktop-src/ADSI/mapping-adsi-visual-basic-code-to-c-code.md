---
title: сопоставление кода Visual Basic ADSI с кодом C++
description: Интерфейсы ADSI состоят из более чем 50 интерфейсов.
ms.assetid: 6316f504-265e-44d4-ba24-e6289065981b
ms.tgt_platform: multiple
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c64a022569a95f38ec1da7a1cb7acf533eb04ca6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172179"
---
# <a name="mapping-adsi-visual-basic-code-to-c-code"></a>сопоставление кода Visual Basic ADSI с кодом C++

Интерфейсы ADSI состоят из более чем 50 интерфейсов. Большинство операций с каталогами можно выполнить, используя только пять интерфейсов. К ним относятся:

-   [**иадсопендсобжект**](/windows/desktop/api/Iads/nn-iads-iadsopendsobject)
-   [**IADs**](/windows/desktop/api/Iads/nn-iads-iads)
-   [**иадсконтаинер**](/windows/desktop/api/Iads/nn-iads-iadscontainer)
-   [**идиректорйобжект**](/windows/desktop/api/Iads/nn-iads-idirectoryobject)
-   [**IDirectorySearch**](/windows/desktop/api/Iads/nn-iads-idirectorysearch)

В следующей таблице перечислены сопоставления из кода ADSI VB/VBS с кодом C++. Имейте в виду, что это не полный список.



| Код VBS                           | Код VC                                                               |
|------------------------------------|-----------------------------------------------------------------------|
| Set obj = GetObject ()              | HR = Адсжетобжект ()                                                   |
| расширением. Установите obj. Получить obj. Источника         | IADs или Идиректорйобжект                                              |
| расширением. Создайте obj. Удалить obj. мовехере | иадсконтаинер                                                         |
| Для каждого... в...                      | Адсбуилденумератор () Адсенумератенекст ()                               |
| Подключение, команда, набор записей     | IDirectorySearch                                                      |
| Дескриптор безопасности, ACL, ACE      | Иадссекуритидескриптор, Иадсакцессконтроллист, Иадсакцессконтролентри |



 

 

 




