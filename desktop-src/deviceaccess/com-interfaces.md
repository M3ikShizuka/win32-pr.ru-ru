---
title: COM-интерфейсы — доступ к устройствам
description: Интерфейсы модели COM в API доступа к устройству.
ms.assetid: 96F532B7-5CF9-4341-932B-7F8BEDA9551F
ms.topic: article
ms.date: 02/11/2020
ms.openlocfilehash: 07abbfd15f8383bbbd9cd9d1f5fc4c9fb1f42b9e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570978"
---
# <a name="com-interfaces---device-access"></a>COM-интерфейсы — доступ к устройствам

Интерфейсы модели COM в API доступа к устройству.

## <a name="in-this-section"></a>В этом разделе

| Раздел | Описание |
|---|---|
| [**икреатедевицеакцессасинк**](/windows/win32/api/Deviceaccess/nn-deviceaccess-icreatedeviceaccessasync)<br/> | Интерфейс [**икреатедевицеакцессасинк**](/windows/win32/api/Deviceaccess/nn-deviceaccess-icreatedeviceaccessasync) возвращается из вызова креатедевицеакцессинстанце. Он позволяет вызывающему объекту управлять операцией привязки к экземпляру устройства, чтобы получить другой интерфейс, который можно использовать для взаимодействия с этим устройством.<br/> |
| [**идевицеиоконтрол**](/windows/win32/api/Deviceaccess/nn-deviceaccess-ideviceiocontrol)<br/> | Отправляет управляющий код в драйвер устройства. Это действие заставляет устройство выполнить соответствующую операцию. <br/> |
| [**идевицерекуесткомплетионкаллбакк**](/windows/win32/api/Deviceaccess/nn-deviceaccess-idevicerequestcompletioncallback)<br/> | Предоставляет метод для управления завершением вызовов метода [**девицеиоконтроласинк**](/windows/win32/api/Deviceaccess/nf-deviceaccess-ideviceiocontrol-deviceiocontrolasync).<br/> |

## <a name="related-topics"></a>Связанные темы

[пример пользовательского доступа к драйверу](https://github.com/microsoftarchive/msdn-code-gallery-microsoft/tree/411c271e537727d737a53fa2cbe99eaecac00cc0/Official%20Windows%20Platform%20Sample/Custom%20driver%20access%20sample), [приложения для устройств UWP для внутренних устройств](/windows-hardware/drivers/devapps/uwp-device-apps-for-specialized-devices), [Центр разработки оборудования](/windows-hardware/drivers/)
