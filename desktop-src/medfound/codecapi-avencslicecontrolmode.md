---
description: 'Задает режим элемента управления "срез". Допустимые значения: 0, 1, и 2.'
ms.assetid: 5269DB79-639C-4F67-B885-BF1274CDB635
title: Свойство CODECAPI_AVEncSliceControlMode (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0aef928a3938b2f0756d2e84b6836da194823dab
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127269307"
---
# <a name="codecapi_avencslicecontrolmode-property"></a>КОДЕКАПИ \_ авенкслицеконтролмоде, свойство

Задает режим элемента управления "срез". Допустимые значения: 0, 1, и 2.

## <a name="data-type"></a>Тип данных

**Ulong** (VT \_ UI4)

## <a name="property-guid"></a>GUID свойства

**КОДЕКАПИ \_ авенкслицеконтролмоде**

## <a name="property-value"></a>Значение свойства

Значения режима элемента управления среза:



| Значение                                                                        | Значение                                                                                                                                                                                                 |
|------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <dl> <dt>0</dt> </dl> | Установка этого значения равным 0 означает, что свойство [кодекапи \_ авенкслицеконтролсизе](codecapi-avencslicecontrolsize.md) будет указывать размер среза в единицах макроблоккс на срез.<br/>     |
| <dl> <dt>1</dt> </dl> | Установка этого значения равным 1 означает, что свойство [кодекапи \_ авенкслицеконтролсизе](codecapi-avencslicecontrolsize.md) будет указывать размер среза в единицах на срез.<br/>            |
| <dl> <dt>2</dt> </dl> | Установка этого значения равным 2 означает, что свойство [кодекапи \_ авенкслицеконтролсизе](codecapi-avencslicecontrolsize.md) будет указывать размер среза в единицах макроблокк строк на срез.<br/> |



 

Кодировщик Возвращает поддерживаемые им значения.

## <a name="remarks"></a>Remarks

**Кодировщики H. 264/AVC:**

Рекомендуется, чтобы кодировщик поддерживал [**GetValue**](/windows/desktop/api/mfobjects/nf-mfobjects-imfmediaevent-getvalue), [**SetValue**](/windows/desktop/api/strmif/nf-strmif-icodecapi-setvalue)и [**жетпараметерранже**](/windows/desktop/api/strmif/nf-strmif-icodecapi-getparameterrange).

Если [**SetValue**](/windows/desktop/api/strmif/nf-strmif-icodecapi-setvalue) не вызывается для кодекапи \_ Авенкслицеконтролмоде, метод [**GetValue**](/windows/desktop/api/mfobjects/nf-mfobjects-imfmediaevent-getvalue) for Кодекапи \_ авенкслицеконтролмоде может возвращать **VFW \_ E \_ кодекапи \_ No \_ Current \_ value**. Параметр [**noreturn может**](/windows/desktop/api/strmif/nf-strmif-icodecapi-getdefaultvalue) возвращать **VFW \_ E \_ кодекапи \_ No \_ по умолчанию** для кодекапи \_ авенкслицеконтролмоде.

Рекомендуемое значение по умолчанию — 2 (размер в МБ на одну строку на срез).

Это статический интерфейс API, что означает, что приложение будет изменяться при выполнении кодировщика.

## <a name="examples"></a>Примеры


```C++
if (pCodecAPI->IsSupported(&CODECAPI_AVEncSliceControlMode) == S_OK) {                
     VARIANT var;
     var.vt = VT_UI4;
     var.ulVal =ulSliceMode;
     pCodecAPI->SetValue(&CODECAPI_AVEncSliceControlMode, &var);
}
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ приложения UWP для классических приложений \|\]<br/>                                   |
| Минимальная версия сервера<br/> | Windows Server 2012 Приложения универсального \[ приложения UWP для настольных приложений \|\]<br/>                        |
| Заголовок<br/>                   | <dl> <dt>Кодекапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> </dl>

 

