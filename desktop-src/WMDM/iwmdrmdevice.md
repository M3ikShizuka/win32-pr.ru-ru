---
title: Интерфейс Ивмдрмдевице
description: Этот интерфейс не предназначен для реализации поставщиком услуг, но предоставляется в целях полной документации. интерфейс ивмдрмдевице позволяет поставщику защищенного содержимого взаимодействовать с устройствами, которые используют Windows Media DRM 10 для портативных устройств.
ms.assetid: ebad4acd-16cc-433f-a5e0-fcae59030f55
keywords:
- Интерфейс Ивмдрмдевице Windows Media диспетчер устройств
- Интерфейс Ивмдрмдевице Windows Media диспетчер устройств, описание
topic_type:
- apiref
api_name:
- IWMDRMDevice
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: ca240f01f552dfdedb0145e49f61f2ead1f18832
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967818"
---
# <a name="iwmdrmdevice-interface"></a>Интерфейс Ивмдрмдевице

Этот интерфейс не предназначен для реализации поставщиком услуг, но предоставляется в целях полной документации.

интерфейс **ивмдрмдевице** позволяет поставщику защищенного содержимого взаимодействовать с устройствами, которые используют Windows Media DRM 10 для портативных устройств.

## <a name="members"></a>Элементы

Интерфейс **ивмдрмдевице** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) . **Ивмдрмдевице** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **ивмдрмдевице** содержит следующие методы.



| Метод                                                                  | Описание                                                                                  |
|:------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [**клеандатасторе**](iwmdrmdevice-cleandatastore.md)                   | Запускает процесс очистки хранилища данных DRM на устройстве.<br/>                  |
| [**жетдевицецертификате**](iwmdrmdevice-getdevicecertificate.md)       | Извлекает сертификат устройства.<br/>                                                 |
| [**жетметерчалленже**](iwmdrmdevice-getmeterchallenge.md)             | Извлекает запрос контроля использования.<br/>                                                 |
| [**жетсекуреклокк**](iwmdrmdevice-getsecureclock.md)                   | Извлекает безопасное время.<br/>                                                       |
| [**жетсекуреклоккчалленже**](iwmdrmdevice-getsecureclockchallenge.md) | Получает запрос на безопасное время.<br/>                                             |
| [**жетсинклист**](iwmdrmdevice-getsynclist.md)                         | Извлекает список синхронизации лицензий.<br/>                                       |
| [**исвмдрмдевице**](iwmdrmdevice-iswmdrmdevice.md)                     | определяет, поддерживает ли устройство Windows Media DRM 10 для переносных устройств.<br/> |
| [**сетлиценсереспонсе**](iwmdrmdevice-setlicenseresponse.md)           | Задает ответ лицензии.<br/>                                                        |
| [**сетметерреспонсе**](iwmdrmdevice-setmeterresponse.md)               | Задает ответ отслеживания.<br/>                                                       |
| [**сетсекуреклоккреспонсе**](iwmdrmdevice-setsecureclockresponse.md)   | Задает отклик на безопасное время.<br/>                                                   |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейсы для поставщиков услуг**](interfaces-for-service-providers.md)
</dt> </dl>

 

