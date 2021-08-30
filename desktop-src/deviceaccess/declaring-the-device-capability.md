---
title: Объявление возможностей устройства
description: В этом разделе объясняется, как объявить GUID возможностей устройства.
ms.assetid: C663F8D2-2CB6-4C3C-A1EB-A3D93AA71FC8
ms.topic: article
ms.date: 02/11/2020
ms.openlocfilehash: d26d41c0f011c21f9f454651adec976a559bdbe20dd75f291404efcd30f2bb5b
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120029084"
---
# <a name="declaring-the-device-capability"></a>Объявление возможностей устройства

В этом разделе объясняется, как объявить GUID возможностей устройства. Все приложения, предназначенные для настраиваемых драйверов, должны объявлять эту возможность.

В манифесте приложения необходимо добавить возможность устройства, как показано ниже.

Это пример объявления возможности для пользовательского устройства. GUID — это идентификатор GUID класса интерфейса устройства.

```XML
<DeviceCapability Name="0B1F1048-B64B-FC9A-CED7-7E4FED3A0DEB" />
```

## <a name="related-topics"></a>Связанные темы

[пример пользовательского доступа к драйверу](https://github.com/microsoftarchive/msdn-code-gallery-microsoft/tree/411c271e537727d737a53fa2cbe99eaecac00cc0/Official%20Windows%20Platform%20Sample/Custom%20driver%20access%20sample), [приложения для устройств UWP для внутренних устройств](/windows-hardware/drivers/devapps/uwp-device-apps-for-specialized-devices), [Центр разработки оборудования](/windows-hardware/drivers/)
