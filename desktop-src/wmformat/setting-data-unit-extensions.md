---
title: Настройка модулей обработки данных
description: Настройка модулей обработки данных
ms.assetid: 28328c9e-8590-48b8-92b6-1c0475978246
keywords:
- Расширенный системный формат (ASF), расширения модулей данных
- ASF (Расширенный системный формат), расширения модулей данных
- расширения модулей данных, Настройка
- потоки, расширения модулей данных
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 822a05a6e6bcbb9f0101d32eed05f2b6c5c68dc8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570206"
---
# <a name="setting-data-unit-extensions"></a>Настройка модулей обработки данных

Некоторые потоки настроены на использование расширений модулей данных для связи дополнительных данных с отдельными примерами. Дополнительные сведения о расширенных примерах см. в разделе [расширения модулей данных](data-unit-extensions.md).

Большинству систем расширения единиц обработки данных требуется расширение для каждого примера в потоке. Если расширение нужного размера не будет предоставлено, модуль записи отклонит пример.

Чтобы добавить Расширенные данные в образец, используйте метод [**INSSBuffer3:: SetProperty**](/previous-versions/windows/desktop/api/Wmsbuffer/nf-wmsbuffer-inssbuffer3-setproperty) . Сведения о расширениях модулей данных, настроенных в потоке, можно получить с помощью методов [**IWMStreamConfig2:: жетдатаунитекстенсионкаунт**](/previous-versions/windows/desktop/api/wmsdkidl/nf-wmsdkidl-iwmstreamconfig2-getdataunitextensioncount) и [**IWMStreamConfig2:: жетдатаунитекстенсион**](/previous-versions/windows/desktop/api/Wmsdkidl/nf-wmsdkidl-iwmstreamconfig2-getdataunitextension) .

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Настройка расширений модуля данных**](configuring-data-unit-extensions.md)
</dt> <dt>

[**Запись файлов ASF**](writing-asf-files.md)
</dt> </dl>

 

 




