---
title: IDeliveryOptimizationJob2 AddFile, метод
description: Метод AddFile добавляет один файл в существующее задание оптимизации доставки.
keywords:
- AddFile - метод
- Метод AddFile, интерфейс IDeliveryOptimizationJob2
- Интерфейс IDeliveryOptimizationJob2, метод AddFile
topic_type:
- apiref
api_name:
- IDeliveryOptimizationJob2.AddFile
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 01/18/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 217215d6f4aaf96de8deab37d08cc492392c0631
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128519896"
---
# <a name="ideliveryoptimizationjob2addfilewithranges-method"></a>Метод IDeliveryOptimizationJob2:: Аддфилевисранжес

Метод AddFile добавляет один файл в существующее задание оптимизации доставки.

## <a name="syntax"></a>Синтаксис

```C++
HRESULT AddFile(
  [in]                              LPCWSTR       fileId,
  [in, unique]                      LPCWSTR       remoteUrl,
  [in]                              DWORD         rangeCount,
  [in, size_is(rangeCount), unique] BG_FILE_RANGE ranges[],
  [in]                              REFIID        riid,
  [out]                             void          **object
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*ИД* \[ для окне\]
</dt> <dd>

Строка идентификатора файла, однозначно определяющая загружаемый файл.

</dd> <dt>

*ремотеурл* \[ окне\]
</dt> <dd>

URL-адрес файла, который оптимизация доставки будет пытаться подключиться для скачивания файла.

</dd> <dt>

*ранжекаунт* \[ окне\]
</dt> <dd>

Количество элементов, содержащихся в *диапазонах*. Нулевое значение означает, что для файла не используются диапазоны.

</dd> <dt>

*диапазоны* \[ окне\]
</dt> <dd>

Необязательный список диапазонов. Каждый диапазон в списке является структурой [**BG_FILE_RANGE**](bg-file-range.md) .

</dd> <dt>

*riid* \[ окне\]
</dt> <dd>

Тип объекта, содержащегося в объекте. Он должен иметь тип IID_IDeliveryOptimizationFile.

</dd> <dt>

*объект* \[ заполняет\]
</dt> <dd>

Объект Иделиверйоптимизатионфиле, представляющий загружаемый файл. 

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает S_OK при успешном или одном из стандартных значений HRESULT при ошибке.

## <a name="requirements"></a>Требования

| Требование | Значение |
|---------------------------|---------------------------------------------------------------------------------|
| Минимальная версия клиента  | Windows 10, только для \[ настольных приложений версии 1803\]                                  |
| Минимальная версия сервера  | Windows Server, только для \[ настольных приложений версии 1709\]                              |
| Заголовок                    | Deliveryoptimization. h                                                          |
| IDL                       | DeliveryOptimization. idl                                                        |
| Библиотека                   | Досвк. lib                                                                       |
| DLL                       | Dosvc.dll                                                                       |
| IID                       | IID_IDeliveryOptimizationJob определяется как EE2584CF-A69C-4848-B633-2649962B3EF7 |

## <a name="see-also"></a>См. также раздел

[**IDeliveryOptimizationJob2**](ideliveryoptimizationjob2.md)
