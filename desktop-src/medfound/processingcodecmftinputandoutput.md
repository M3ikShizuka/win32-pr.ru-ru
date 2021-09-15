---
description: Обработка входных и выходных файлов MFT кодека
ms.assetid: 2d012508-de13-411f-9102-22e47faddffd
title: Обработка входных и выходных файлов MFT кодека
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 1af3a16fa1855574f1b7618bc0d41bf85c15412f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461995"
---
# <a name="processing-codec-mft-input-and-output"></a>Обработка входных и выходных файлов MFT кодека

После настройки типа входных данных и типа выходных данных для MFT можно начать обработку образцов данных. Передайте образцы в таблицу MFT для обработки с помощью метода [**имфтрансформ::P роцессинпут**](/windows/desktop/api/mftransform/nf-mftransform-imftransform-processinput) , а затем извлеките обработанный пример, вызвав [**Имфтрансформ::P роцессаутпут**](/windows/desktop/api/mftransform/nf-mftransform-imftransform-processoutput). Необходимо задать точные метки времени и длительности для всех пройденных выборок. Метки времени не являются строго необходимыми, но помогают поддерживать синхронизацию аудио и видео. Если у вас нет меток времени для выборки, лучше оставить их, не используя неопределенные значения.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Работа с кодеками МФТС](workingwithcodecmfts.md)
</dt> </dl>

 

 



