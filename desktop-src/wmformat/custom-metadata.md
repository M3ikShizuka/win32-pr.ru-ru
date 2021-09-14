---
title: Пользовательские метаданные
description: Пользовательские метаданные
ms.assetid: 86132163-da56-416a-9539-874d18972932
keywords:
- Windows Пакет SDK для формата мультимедиа, пользовательские метаданные
- Расширенный системный формат (ASF), пользовательские метаданные
- ASF (Расширенный системный формат), пользовательские метаданные
- Windows Пакет SDK для формата мультимедиа, интерфейс IWMHeaderInfo3
- Расширенный системный формат (ASF), интерфейс IWMHeaderInfo3
- ASF (Расширенный системный формат), интерфейс IWMHeaderInfo3
- метаданные, Настройка
- IWMHeaderInfo3
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a795ab184e5bd6120278f61c0d3654679fd79c28
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127256345"
---
# <a name="custom-metadata"></a>Пользовательские метаданные

помимо множества поддерживаемых атрибутов, поставляемых с пакетом SDK для Windows Media Format, можно создать атрибуты метаданных для собственных спецификаций. При создании пользовательских атрибутов метаданных следует использовать легко узнаваемое соглашение об именовании, чтобы избежать возможного конфликта с атрибутами, созданными другими пользователями.

Рекомендуется использовать методы [**IWMHeaderInfo3**](/previous-versions/windows/desktop/api/wmsdkidl/nn-wmsdkidl-iwmheaderinfo3) для создания метаданных из-за дополнительной гибкости, предоставляемой методам [**ивмхеадеринфо**](/previous-versions/windows/desktop/api/wmsdkidl/nn-wmsdkidl-iwmheaderinfo).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Атрибуты**](attributes.md)
</dt> <dt>

[**Компоненты метаданных**](metadata-features.md)
</dt> <dt>

[**Работа с метаданными**](working-with-metadata.md)
</dt> </dl>

 

 




