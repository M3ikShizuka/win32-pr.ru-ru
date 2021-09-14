---
description: Получает метрики качества при отмене акустического эха (AEC) из схемы DSP для записи голоса.
ms.assetid: de2e86ae-0469-471f-9105-0bb38a59b428
title: Свойство MFPKEY_WMAAECMA_QUALITY_METRICS (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a3740630bc23c4e3e0e824e55b4e34bcd8b1347f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127268803"
---
# <a name="mfpkey_wmaaecma_quality_metrics-property"></a>\_ \_ Свойство МЕТРИК качества мфпкэй вмааекма \_

Получает метрики качества при отмене акустического эха (AEC) из схемы DSP для записи голоса.

## <a name="constant-for-ipropertybag"></a>Константа для Ипропертибаг

Доступно только с помощью [**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore).

## <a name="data-type"></a>Тип данных

\_большой двоичный объект VT

## <a name="remarks"></a>Remarks

Значением этого свойства является структура [ \_ структуры аеккуалитиметрикс](/windows/win32/api/wmcodecdsp/ns-wmcodecdsp-aecqualitymetrics_struct) . Это свойство доступно только для чтения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                    |
| Заголовок<br/>                   | <dl> <dt>Вмкодекдсп. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> <dt>

[DSP для записи речи](voicecapturedmo.md)
</dt> </dl>

 

 
