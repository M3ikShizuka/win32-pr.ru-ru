---
description: Управляет сигнализацией Мфсампликстенсион \_ меанабсолутедифференце через имфаттрибуте для каждого выходного образца.
ms.assetid: 61C0F431-FBF5-4B17-8F3A-0F6AD2BA33B7
title: Свойство CODECAPI_AVEncVideoMeanAbsoluteDifference (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f58a7bc0da9fce88c0b8137d800d527d4717801c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127269256"
---
# <a name="codecapi_avencvideomeanabsolutedifference-property"></a>КОДЕКАПИ \_ авенквидеомеанабсолутедифференце, свойство

Управляет сигнализацией [мфсампликстенсион \_ Меанабсолутедифференце](mfsampleextension-meanabsolutedifference.md) через [**имфаттрибуте**](/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes) для каждого выходного образца.

## <a name="data-type"></a>Тип данных

**Ulong** (VT \_ UI4)

## <a name="property-guid"></a>GUID свойства

**КОДЕКАПИ \_ авенквидеомеанабсолутедифференце**

## <a name="remarks"></a>Remarks

Если приложение устанавливает ненулевое значение, кодировщику следует добавить к каждому выходному примеру атрибут [мфсампликстенсион \_ меанабсолутедифференце](mfsampleextension-meanabsolutedifference.md) Sample. Атрибут Мфсампликстенсион \_ меанабсолутедифференце показывает среднее абсолютное различие между исходными примерами и прогнозируемыми примерами на плоскости Y.

Если кодировщик возвращает 0 для **жетпараметерранже**, кодировщик не поддерживает выходные данные [мфсампликстенсион \_ меанабсолутедифференце](mfsampleextension-meanabsolutedifference.md) в выходных образцах.

Значение по умолчанию должно быть равно 0.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Кодекапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> </dl>

 

 




