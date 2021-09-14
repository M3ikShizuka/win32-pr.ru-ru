---
description: Метод Жетсубпиктурелангуаже извлекает язык для указанного потока субтитров.
ms.assetid: 2a2e6961-99c3-4200-b462-b381f9e37066
title: Метод Жетсубпиктурелангуаже
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8f87d1bf95ee13a1a15e631e2bc53477b62b789a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053353"
---
# <a name="getsubpicturelanguage-method"></a>Метод Жетсубпиктурелангуаже

> [!Note]  
> этот компонент доступен для использования в операционных системах Microsoft Windows 2000, Windows XP и Windows Server 2003. В последующих версиях он может быть изменен или недоступен.

 

`GetSubpictureLanguage`Метод получает язык для указанного потока субтитров.

``` syntax
[ sLang = ] MSWebDVD.GetSubpictureLanguage(iStream)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="iStream"></span><span id="istream"></span><span id="ISTREAM"></span>*iStream*
</dt> <dd>

Указывает номер потока субтитров, язык текста которого требуется получить в виде целого числа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает читаемую строку, идентифицирующую язык аудиопотока в текущем заголовке.

 

 



