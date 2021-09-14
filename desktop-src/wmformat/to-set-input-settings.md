---
title: установка входных Параметры
description: установка входных Параметры
ms.assetid: 288801a7-793f-43bd-9c5a-f9e1bd86ecc3
keywords:
- Расширенный формат систем (ASF), параметры ввода
- ASF (Расширенный системный формат), параметры ввода
- профили, параметры ввода
- кодеки, параметры ввода
- потоки, параметры ввода
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4e7b2db64a7346cc8b9d46c48f0add79dafcac95
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127247243"
---
# <a name="to-set-input-settings"></a>установка входных Параметры

Основные свойства входного носителя и потока мультимедиа определяются структурой [**типа WM \_ Media \_**](/previous-versions/windows/desktop/api/wmsdkidl/ns-wmsdkidl-wm_media_type) . Для входных форматов данные типа мультимедиа задаются приложением. Для форматов потока сведения о типе мультимедиа задаются в профиле, который назначается модулю записи. Некоторые свойства не зависят от типа мультимедиа и должны быть заданы для входных данных перед началом записи. Эти свойства являются компонентами кодека и модуля записи, которые не зависят от типа потока, и должны быть заданы после назначения профиля в модуле записи, но перед началом записи.

Для установки входного параметра требуется вызов [**IWMWriterAdvanced2:: сетинпутсеттинг**](/previous-versions/windows/desktop/api/Wmsdkidl/nf-wmsdkidl-iwmwriteradvanced2-setinputsetting). Можно также проверить текущее значение параметра с помощью вызова [**IWMWriterAdvanced2:: жетинпутсеттинг**](/previous-versions/windows/desktop/api/Wmsdkidl/nf-wmsdkidl-iwmwriteradvanced2-getinputsetting).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Использование профилей с модулем записи**](to-use-profiles-with-the-writer.md)
</dt> <dt>

[**Запись файлов ASF**](writing-asf-files.md)
</dt> <dt>

[**запись образа Потоки**](writing-image-streams.md)
</dt> </dl>

 

 




