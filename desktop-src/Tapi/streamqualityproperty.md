---
description: 'Перечисление Стреамкуалитипроперти, используемое методами Итстреамкуалитиконтрол::, Итстреамкуалитиконтрол:: Get и Итстреамкуалитиконтрол:: Set для указания свойства качества потока, для которого выполняется обращение.'
ms.assetid: 28c9257f-6fbb-440f-9b84-c15a74229b5b
title: Перечисление Стреамкуалитипроперти (Ипмсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7f552641cd0847bb3ff8eec9d528a03171a78c2e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127374772"
---
# <a name="streamqualityproperty-enumeration"></a>Перечисление Стреамкуалитипроперти

\[это перечисление недоступно для использования в Windows Vista, Windows Server 2008 и последующих версиях операционной системы. API клиента RTC предоставляет аналогичные функциональные возможности.\]

Перечисление **стреамкуалитипроперти** , используемое методами [**итстреамкуалитиконтрол::**](itstreamqualitycontrol-getrange.md), [**Итстреамкуалитиконтрол:: Get**](itstreamqualitycontrol-get.md)и [**итстреамкуалитиконтрол:: Set**](itstreamqualitycontrol-set.md) для указания свойства качества потока, для которого выполняется обращение.

## <a name="syntax"></a>Синтаксис


```C++
} StreamQualityProperty;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="StreamQuality_MaxBitrate"></span><span id="streamquality_maxbitrate"></span><span id="STREAMQUALITY_MAXBITRATE"></span>**Стреамкуалити \_ максбитрате**
</dt> <dd>

Максимальная скорость.

</dd> <dt>

<span id="StreamQuality_CurrBitrate"></span><span id="streamquality_currbitrate"></span><span id="STREAMQUALITY_CURRBITRATE"></span>**Стреамкуалити \_ куррбитрате**
</dt> <dd>

Минимальная скорость.

</dd> <dt>

<span id="StreamQuality_MinFrameInterval"></span><span id="streamquality_minframeinterval"></span><span id="STREAMQUALITY_MINFRAMEINTERVAL"></span>**Стреамкуалити \_ минфрамеинтервал**
</dt> <dd>

Максимальный интервал кадров.

</dd> <dt>

<span id="StreamQuality_AvgFrameInterval"></span><span id="streamquality_avgframeinterval"></span><span id="STREAMQUALITY_AVGFRAMEINTERVAL"></span>**Стреамкуалити \_ авгфрамеинтервал**
</dt> <dd>

Минимальный интервал кадров.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------|------------------------------------------------------------------------------------|
| Версия TAPI<br/> | Требуется TAPI 3,1<br/>                                                       |
| Заголовок<br/>       | <dl> <dt>Ипмсп. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Итстреамкуалитиконтрол:: Range**](itstreamqualitycontrol-getrange.md)
</dt> <dt>

[**Итстреамкуалитиконтрол:: Get**](itstreamqualitycontrol-get.md)
</dt> <dt>

[**Итстреамкуалитиконтрол:: Set**](itstreamqualitycontrol-set.md)
</dt> </dl>

 

 




