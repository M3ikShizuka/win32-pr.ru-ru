---
description: Указывает максимальный поддерживаемый кодировщиком обработчик запросов.
ms.assetid: 2C02F82B-E645-4C5B-9526-5E130A6E2F67
title: Свойство CODECAPI_AVEncVideoMaxQP (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d9bcf23866da5530d2edc1203be359071e5e33e7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127269259"
---
# <a name="codecapi_avencvideomaxqp-property"></a>КОДЕКАПИ \_ авенквидеомакскп, свойство

Указывает максимальный поддерживаемый кодировщиком обработчик запросов.

## <a name="data-type"></a>Тип данных

**Ulong** (VT \_ UI4)

## <a name="property-guid"></a>GUID свойства

**КОДЕКАПИ \_ авенквидеомакскп**

## <a name="remarks"></a>Remarks

**Кодировщики H. 264/AVC:**

Кодировщик должен поддерживать [**GetValue**](/windows/desktop/api/mfobjects/nf-mfobjects-imfmediaevent-getvalue), [**SetValue**](/windows/desktop/api/strmif/nf-strmif-icodecapi-setvalue)и [**жетпараметерранже**](/windows/desktop/api/strmif/nf-strmif-icodecapi-getparameterrange).

Это статическое свойство означает, что его можно задать только до начала сеанса кодирования.

Значение по умолчанию должно быть максимальным числом запросов QP, разрешенным соответствующим стандартом кодирования. Например, кодировщики H. 264 должны иметь значение по умолчанию 51.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ приложения UWP для классических приложений \|\]<br/>                                   |
| Минимальная версия сервера<br/> | Windows Server 2012 Приложения универсального \[ приложения UWP для настольных приложений \|\]<br/>                        |
| Заголовок<br/>                   | <dl> <dt>Кодекапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> <dt>

[КОДЕКАПИ \_ авенквидеоминкп](codecapi-avencvideominqp.md)
</dt> </dl>

 

