---
title: Интерфейс IDeliveryOptimizationFile2
description: IDeliveryOptimizationFile2 поддерживает настройку и получение необязательных свойств файла.
keywords:
- Интерфейс IDeliveryOptimizationFile2
- Интерфейс IDeliveryOptimizationFile2, описание
topic_type:
- apiref
api_name:
- IDeliveryOptimizationFile2
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 01/18/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 7e5ef827758e054ed391303a283b490e0db66d3b
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128520051"
---
# <a name="ideliveryoptimizationfile2-interface"></a>Интерфейс IDeliveryOptimizationFile2

**IDeliveryOptimizationFile2** поддерживает настройку и получение необязательных свойств файла. 

## <a name="members"></a>Элементы

Интерфейс **IDeliveryOptimizationFile2** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) . **IDeliveryOptimizationFile2** также имеет следующие типы членов:

- [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **IDeliveryOptimizationFile2** содержит следующие методы.

| Метод                                                 | Описание                                                  |
|:-------------------------------------------------------|:-------------------------------------------------------------|
| [**GetProperty**](ideliveryoptimizationfile2-getproperty.md)  | Этот метод возвращает одно свойство файла оптимизации доставки. |
| [**SetProperty**](ideliveryoptimizationfile2-setproperty.md)  | Этот метод задает одно свойство файла оптимизации доставки.    |

## <a name="requirements"></a>Требования

| Требование | Значение |
|-------------------------------|-----------------------------------------------------------------------------------|
| Минимальная версия клиента      | Windows 10, только для \[ настольных приложений версии 1803\]                                    |
| Минимальная версия сервера      | Windows Server, только для \[ настольных приложений версии 1709\]                                |
| Заголовок                        | Deliveryoptimization. h                                                            |
| IDL                           | DeliveryOptimization. idl                                                          |
| Библиотека                       | Досвк. lib                                                                         |
| DLL                           | Dosvc.dll                                                                         |
| IID                           | IID_IDeliveryOptimizationFile2 определен как 3A87296F-6EC2-4126-AB29-E3F8DC4CC390 |
