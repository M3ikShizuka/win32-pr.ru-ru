---
title: Перечисление Додовнлоадпропертекс
description: Указывает идентификатор расширенных свойств для операции скачивания для оптимизации доставки.
keywords:
- Перечисление Додовнлоадпропертекс, Додовнлоадпропертекс
topic_type:
- apiref
api_name:
- DODownloadPropertyEx
api_location:
- deliveryoptimizationdownloadtypes.h
api_type:
- HeaderDef
ms.localizationpriority: low
ms.topic: reference
ms.date: 07/29/2019
ms.openlocfilehash: c6a0f130aad68eab08a577b0153648cf17547189
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128521006"
---
# <a name="dodownloadpropertyex-enumeration"></a>Перечисление Додовнлоадпропертекс

> [!IMPORTANT]
> Перечисление **додовнлоадпропертекс** является устаревшим. Вместо этого используйте перечисление [додовнлоадпроперти](../deliveryoptimizationdownloadtypes/ne-deliveryoptimizationdownloadtypes-dodownloadproperty.md) с [идодовнлоад::](../do/nf-do-idodownload-getproperty.md) и [идодовнлоад:: SetProperty](../do/nf-do-idodownload-setproperty.md).

Перечисление **додовнлоадпропертекс** указывает идентификатор расширенных свойств для операции скачивания для оптимизации доставки. Это перечисление используется интерфейсом **идодовнлоадинтернал** , а значение **типа Variant** используется для получения и задания значения свойства.

## <a name="syntax"></a>Синтаксис

```cpp
typedef enum _DODownloadPropertyEx
{
  DODownloadPropertyEx_UpdateId = 0,
  DODownloadPropertyEx_CorrelationVector,
  DODownloadPropertyEx_DecryptionInfo,    
  DODownloadPropertyEx_IntegrityCheckInfo,   
  DODownloadPropertyEx_IntegrityCheckMandatory, 
  DODownloadPropertyEx_TotalSizeBytes, 
  DODownloadPropertyEx_TempLocalFileUsage 
} DODownloadPropertyEx;
```
## <a name="constants"></a>Константы

| Требование | Значение |
|-|-|
| DODownloadPropertyEx_UpdateId | Зарезервировано. Не используется. |
| DODownloadPropertyEx_CorrelationVector | Необязательный элемент. Задает конкретный вектор корреляции для телеметрии. Тип VARIANT — VT_BSTR. |
| DODownloadPropertyEx_DecryptionInfo | Зарезервировано. Не используется. |
| DODownloadPropertyEx_IntegrityCheckInfo | Необязательный только для записи. Задает расположение файла хэш-кода (ФФ), которое используется при оптимизации доставки для выполнения проверок целостности во время выполнения для загруженного содержимого. Тип VARIANT — VT_BSTR. |
| DODownloadPropertyEx_IntegrityCheckMandatory | Необязательный элемент. Задает логический флаг, указывающий, является ли использование хэш-файла фрагмента (ФФ) обязательным. Если VARIANT_TRUE, загрузка будет прервана после сбоя проверки целостности. Тип VARIANT — VT_BOOL. |
| DODownloadPropertyEx_TotalSizeBytes | Зарезервировано. Не используется. |
| DODownloadPropertyEx_TempLocalFileUsage | Зарезервировано. Не используется. |

## <a name="requirements"></a>Требования

| &nbsp; | &nbsp; |
| ---- |:---- |
| **Минимальная версия клиента** | Windows 10, версия 1809 \[ Только приложения Win32\] |
| **Минимальная версия сервера** | Windows Сервер, \[ только приложения Win32 версии 1809\] |
| **Header** | Додовнлоадинтернал. h |
