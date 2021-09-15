---
description: у меня есть файл AVI, содержащий поток видео Windows Media.
ms.assetid: 0b4c5bf2-caa6-4e14-be5f-9e25ec918cf0
title: у меня есть файл AVI, содержащий поток видео Windows Media. Как преобразовать его в WMV-файл?
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 08c770a8355e92c6cfe052d86a17c6638a7a9948
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462220"
---
# <a name="i-have-an-avi-file-containing-a-windows-media-video-stream-how-can-i-convert-it-to-a-wmv-file"></a>у меня есть файл AVI, содержащий поток видео Windows Media. Как преобразовать его в WMV-файл?

интерфейсы кодеков Windows Media Audio и Video не предоставляют методы для создания файлов с использованием формата ASF, который используется для файлов WMV. если требуется преобразовать файл (с помощью любого контейнера) в файл ASF, необходимо использовать объекты пакета SDK Windows Media Format.

получите сжатые Windows примеры мультимедиа из исходного файла и передайте их в объект модуля записи как образцы потока. дополнительные сведения см. в документации по пакету SDK для серии Windows Media Format 9.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Часто задаваемые вопросы](frequentlyaskedquestions.md)
</dt> </dl>

 

 



