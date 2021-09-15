---
description: Определяет один метод обратного вызова.
ms.assetid: 579f7a29-cd98-4d97-9f8e-9b786897df1c
title: Интерфейс Иконнектионрекуесткаллбакк (Девпкэй. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IConnectionRequestCallback
api_type:
- COM
api_location:
- PortableDeviceGuids.lib
- PortableDeviceGuids.dll
ms.openlocfilehash: aca827de068ce221f013f03b35f88fd76a030dd4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570139"
---
# <a name="iconnectionrequestcallback-interface"></a>Интерфейс Иконнектионрекуесткаллбакк

Интерфейс **иконнектионрекуесткаллбакк** определяет один метод обратного вызова. приложение Windows Portable devices (WPD) реализует этот необязательный интерфейс модели COM для получения уведомлений о завершенных запросах и отмены ожидающих запросов. запросы отправляются с помощью методов [**ипортабледевицеконнектор:: Подключение**](/windows/desktop/api/portabledeviceconnectapi/nf-portabledeviceconnectapi-iportabledeviceconnector-connect) и [**ипортабледевицеконнектор::D соединения**](/windows/desktop/api/portabledeviceconnectapi/nf-portabledeviceconnectapi-iportabledeviceconnector-disconnect) .

## <a name="members"></a>Элементы

Интерфейс **иконнектионрекуесткаллбакк** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) . **Иконнектионрекуесткаллбакк** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **иконнектионрекуесткаллбакк** содержит следующие методы.



| Метод                                                      | Описание                                                                           |
|:------------------------------------------------------------|:--------------------------------------------------------------------------------------|
| [**OnComplete**](iconnectionrequestcallback-oncomplete.md) | Уведомляет приложение о завершении ранее запланированного запроса.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                                                                                                             |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                                                                              |
| Заголовок<br/>                   | <dl> <dt>Девпкэй. h; </dt> <dt>Портабледевицеконнектапи. h</dt> </dl> |
| IDL<br/>                      | <dl> <dt>Портабледевицеконнектапи. idl</dt> </dl>                                                                |
| Библиотека<br/>                  | <dl> <dt>Портабледевицегуидс. lib</dt> </dl>                                                                     |



 

