---
description: Пример Вавсинк
ms.assetid: 9e1af25f-d55c-45db-8c76-abf814e16700
title: Пример Вавсинк
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3e96ecca551b6ea3e6837f211f0afcb34818d635
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127363616"
---
# <a name="wavsink-sample"></a>Пример Вавсинк

Показывает, как реализовать пользовательский приемник мультимедиа в Microsoft Media Foundation. В примере реализуется приемник архива, записывающий несжатый аудиопоток PCM в WAV-файл.

## <a name="apis-demonstrated"></a>Продемонстрированные API

В этом образце демонстрируются следующие интерфейсы Media Foundation:

-   [**имфклоккстатесинк**](/windows/desktop/api/mfidl/nn-mfidl-imfclockstatesink)
-   [**имффинализаблемедиасинк**](/windows/desktop/api/mfidl/nn-mfidl-imffinalizablemediasink)
-   [**имфмедиасинк**](/windows/desktop/api/mfidl/nn-mfidl-imfmediasink)
-   [**имфмедиатипехандлер**](/windows/desktop/api/mfidl/nn-mfidl-imfmediatypehandler)
-   [**имфстреамсинк**](/windows/desktop/api/mfidl/nn-mfidl-imfstreamsink)

## <a name="usage"></a>Использование

пример вавсинк содержит два Visual Studioных проекта:

-   Вавсинк. vcproj строит статическую библиотеку, которая содержит реализацию приемника мультимедиа.
-   Вритевавфиле. vcproj создает консольное приложение, использующее приемник мультимедиа для создания WAV-файла. Это приложение связывается с библиотекой, созданной проектом Вавсинк.

## <a name="requirements"></a>Требования



| Продукт                                                        | Version   |
|----------------------------------------------------------------|-----------|
| [Windows SDK](https://msdn.microsoft.com/windowsvista/bb980924.aspx) | Windows 7 |



 

## <a name="downloading-the-sample"></a>Загрузка образца

этот пример доступен в [репозитории github для классических примеров Windows](https://github.com/Microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/multimedia/mediafoundation/wavsink).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Примеры пакетов SDK Media Foundation](media-foundation-sdk-samples.md)
</dt> <dt>

[Приемники носителей](media-sinks.md)
</dt> </dl>

 

 



