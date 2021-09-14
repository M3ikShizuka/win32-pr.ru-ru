---
description: Сведения о ссылках на параметры и элемент Параметердеф. Примером параметра, включающего элемент ParameterRef, является пользовательский параметр размера носителя.
ms.assetid: 2c796d5c-1556-4348-83e2-23e93780ebc1
title: Создание ссылок на параметры
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 650790af5ca6849bd082b4819dd4c411adea320f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343642"
---
# <a name="referencing-parameters"></a>Создание ссылок на параметры

Этот раздел не является актуальным. Самые актуальные сведения см. в [спецификации печати схемы](https://download.microsoft.com/download/D/E/C/DECA6E6B-3E81-48E7-B7EF-6D92A547D03C/print-schema-spec-2-0.zip).

Конкретный пример параметра, включающего элемент ParameterRef, — это пользовательский параметр размера носителя. Обратите внимание, что он ссылается на два параметра: Пажемедиасиземедиасизевидс и Пажемедиасиземедиасизехеигхт. Каждый экземпляр ParameterRef ссылается на экземпляр Параметердеф, который определен в любом расположении документа PrintCapabilities. Дополнительные сведения об элементе Параметердеф см. в разделе [параметердеф](parameterdef.md). Основные сведения об определении параметров см. в разделе [элементы параметердеф и параметеринит](parameterdef-and-parameterinit-elements.md).

``` syntax
<!--Example of ParamterRef usage within a Feature-->
<psf:Option name="psk:CustomMediaSize" constrained="psk:None">
  <psf:ScoredProperty name="psk:MediaSizeWidth">
    <psf:ParameterRef name="psk:PageMediaSizeMediaSizeWidth" />
  </psf:ScoredProperty>
  <psf:ScoredProperty name="psk:MediaSizeHeight">
    <psf:ParameterRef name="psk:PageMediaSizeMediaSizeHeight" />
  </psf:ScoredProperty>
</psf:Option>
```

Просто создать параметризованный параметр недостаточно, чтобы убедиться, что параметр будет обрабатываться и обрабатываться правильно. Поставщик PrintCapabilities/PrintTicket и клиенты должны предоставить дополнительную поддержку для правильной реализации параметризованных экземпляров параметров. Необходимые поведения описаны в следующих разделах.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Печать спецификации схемы](https://download.microsoft.com/download/D/E/C/DECA6E6B-3E81-48E7-B7EF-6D92A547D03C/print-schema-spec-2-0.zip)
</dt> </dl>

 

 



