---
title: Доступ к метаданным и атрибутам в приложении
description: Получение и установка метаданных и атрибутов в приложении
ms.assetid: 308a722d-1c65-41eb-a0e2-21171eb410d5
keywords:
- Windows Диспетчер устройств мультимедиа, метаданные
- Диспетчер устройств, метаданные
- инструкции по программированию, метаданные
- Классические приложения, метаданные
- создание Windows мультимедиа диспетчер устройств приложений, метаданные
- метаданные
- Windows Диспетчер устройств мультимедиа, атрибуты
- Диспетчер устройств, атрибуты
- инструкции по программированию, атрибуты
- Классические приложения, атрибуты
- создание Windows мультимедиа диспетчер устройств приложений, атрибуты
- attributes
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6a78dbb31ebcc5ec99b1db3503b386b09b5a3c05
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967869"
---
# <a name="accessing-metadata-and-attributes-in-the-app"></a>Доступ к метаданным и атрибутам в приложении

Общие сведения о метаданных и атрибутах доступны в статье [Получение и установка метаданных и атрибутов](getting-and-setting-metadata-and-attributes.md). В этом разделе рассматриваются определенные вызовы методов приложений для получения или задания значений.

Приложения могут извлекать атрибуты или метаданные о конкретном хранилище путем вызова [**ивмдмстораже:: InAttribute**](/windows/desktop/api/mswmdm/nf-mswmdm-iwmdmstorage-getattributes), [**IWMDMStorage2:: GetAttributes2**](/windows/desktop/api/mswmdm/nf-mswmdm-iwmdmstorage2-getattributes2), [**IWMDMStorage3::-Metadata**](/windows/desktop/api/mswmdm/nf-mswmdm-iwmdmstorage3-getmetadata) или [**IWMDMStorage4:: жетспеЦифиедметадата**](/windows/desktop/api/mswmdm/nf-mswmdm-iwmdmstorage4-getspecifiedmetadata). Параметр- **Metadata** извлекает полную коллекцию всех метаданных, связанных с хранилищем, и приложение может перечислить все значения или запросить определенные значения из коллекции. **ЖетспеЦифиедметадата** создает объект метаданных от имени вызывающего объекта. вызывающий объект может запросить подмножество доступных данных, заполнив параметр *ппвсзпропнамес* массивом требуемых Windows Media диспетчер устройств строк свойств и количеством этого массива. Возвращенный объект метаданных будет заполнен этими свойствами, которые можно получить. Эти свойства, которые не удалось получить, будут отсутствовать. Метаданные возвращаются на основе наилучшей силы.

Устройство может устанавливать атрибуты или метаданные в хранилище путем вызова [**ивмдмстораже:: сетаттрибутес**](/windows/desktop/api/mswmdm/nf-mswmdm-iwmdmstorage-setattributes), [**IWMDMStorage2:: SetAttributes2**](/windows/desktop/api/mswmdm/nf-mswmdm-iwmdmstorage2-setattributes2)или [**IWMDMStorage3:: сетметадата**](/windows/desktop/api/mswmdm/nf-mswmdm-iwmdmstorage3-setmetadata). Обратите внимание, что не существует гарантии, что все значения будут сохранены, так как они могут храниться в непостоянном внешнем хранилище файлов, они могут не поддерживаться или устройство может не поддерживать доступ к свойствам в качестве записываемых.

Также можно получить или задать метаданные о устройстве, вызвав [**IWMDMDevice3::-Property**](/windows/desktop/api/mswmdm/nf-mswmdm-iwmdmdevice3-getproperty) или [**IWMDMDevice3:: SetProperty**](/windows/desktop/api/mswmdm/nf-mswmdm-iwmdmdevice3-setproperty). Существует отдельная таблица констант метаданных устройства, перечисленных в конце [констант метаданных](metadata-constants.md).

Примеры использования этих методов приведены в справочной документации по каждому методу.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**создание Windows мультимедиа диспетчер устройств приложение**](creating-a-windows-media-device-manager-application.md)
</dt> <dt>

[**Получение и установка метаданных и атрибутов**](getting-and-setting-metadata-and-attributes.md)
</dt> </dl>

 

 




