---
title: Интерфейс IDeliveryOptimizationJob2
description: 'Дополнительные сведения о: интерфейс IDeliveryOptimizationJob2'
keywords:
- Интерфейс IDeliveryOptimizationJob2
topic_type:
- apiref
api_name:
- IDeliveryOptimizationJob2
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 01/18/2019
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 7868dc29a746566291a10f6b8f8854f33fe2221f
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128521191"
---
# <a name="ideliveryoptimizationjob2-interface"></a>Интерфейс IDeliveryOptimizationJob2

IDeliveryOptimizationJob2 позволяет добавить один файл в задание загрузки и немедленно получить его. Этот интерфейс также поддерживает настройку и получение дополнительных свойств задания.

## <a name="members"></a>Элементы

Интерфейс **IDeliveryOptimizationJob2** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) . **IDeliveryOptimizationJob2** также имеет следующие типы членов:

- [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **IDeliveryOptimizationJob2** содержит следующие методы.

| Метод                                              | Описание                                                          |
|:----------------------------------------------------|----------------------------------------------------------------------|
| [**AddFile**](ideliveryoptimizationjob2-addfile.md) | Метод AddFile добавляет один файл в существующее задание оптимизации доставки.         |
| [**GetProperty**](ideliveryoptimizationjob2-getproperty.md) | Метод AddFile добавляет один файл в существующее задание оптимизации доставки. |
| [**SetProperty**](ideliveryoptimizationjob2-setproperty.md) | Этот метод не используется.                                       |

## <a name="requirements"></a>Требования

| Требование | Значение |
|--------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента | Windows 10, только для \[ настольных приложений версии 1803\]                                   |
| Минимальная версия сервера | Windows Server, только для \[ настольных приложений версии 1709\]                               |
| Заголовок                   | Deliveryoptimization. h                                                           |
| IDL                      | DeliveryOptimization. idl                                                         |
| Библиотека                  | Досвк. lib                                                                        |
| DLL                      | Dosvc.dll                                                                        |
| IID                      | IID_IDeliveryOptimizationJob2 определен как 18995A26-BF59-4ABE-9F8B-D5092D5A2405 |
