---
title: Выбор файлов
description: Выбор файлов
ms.assetid: dfa44a32-7d72-47f7-a872-33b823a34798
keywords:
- Создание обложек, выбор файлов
- обложки проигрыватель Windows Media, выбор файлов
- обложки, выбор файлов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2ed90a5813880c87dbaf297808cc79c65ed066eb1585ba63ddd97d0305199230
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119764254"
---
# <a name="choosing-files"></a>Выбор файлов

Если вы хотите выбрать файл, можно использовать код, похожий на пример списка воспроизведения, но заменить следующие сведения в разделе ПЛАЙЕЛЕМЕНТ:


```C++
<PLAYELEMENT
  mappingColor = "#00FF00"
  onClick = "JScript:player.URL=theme.openDialog('FILE_OPEN','FILES_ALL');"
  />

```



Эта строка будет использовать метод **Опендиалог** **темы** для определения **URL-адреса** проигрывателя. Его можно использовать для выбора файлов, отсутствующих в списках воспроизведения.

Аналогичный пример рабочего **опендиалог** см. в разделе примера пакета SDK.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Руководством по созданию обложки**](skin-creation-guide.md)
</dt> </dl>

 

 




