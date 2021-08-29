---
title: Ивмпкдромрип Риппрогресс, свойство
description: Свойство Риппрогресс получает сведения о ходе копирования компакт-диска в процентах завершения.
ms.assetid: 00d4f074-a16d-4c5f-930f-4411b90303f1
keywords:
- проигрыватель Windows Media свойства риппрогресс
- проигрыватель Windows Media свойства риппрогресс, интерфейс ивмпкдромрип
- проигрыватель Windows Media интерфейса ивмпкдромрип, свойство риппрогресс
topic_type:
- apiref
api_name:
- IWMPCdromRip.ripProgress
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ea0d80a9eeed0246c48c142177bb4611c8666ca8b4f783d51f472dada2bbdbc5
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119246754"
---
# <a name="iwmpcdromripripprogress-property"></a>Свойство Ивмпкдромрип:: Риппрогресс

Свойство **риппрогресс** получает сведения о ходе копирования компакт-диска в процентах завершения.

## <a name="syntax"></a>Синтаксис


```CSharp
public System.Int32 ripProgress {get; set;}
```


```VB

Public ReadOnly Property ripProgress As System.Int32
```





## <a name="property-value"></a>Значение свойства

Значение **System. Int32** , которое является значением хода выполнения. Значения хода выполнения находятся в диапазоне от 0 до 100.

## <a name="remarks"></a>Remarks

Значение Progress представляет завершенный процент всего процесса копирования. Чтобы определить ход выполнения определенной записи, используйте [ивмпмедиа. getItemInfo](wmplibiwmpplaylist-iwmpplaylist-getiteminfo--vb-and-c.md) с **риппрогресс** в качестве имени атрибута. Чтобы получить индекс дорожки, скопированной в данный момент, вызовите Ивмпплайлист. getItemInfo с именем атрибута "Куррентриптраккиндекс".

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 11.<br/>                                                                                    |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ивмпкдромрип (VB и C#)**](iwmpcdromrip--vb-and-c.md)
</dt> <dt>

[**Копирование компакт-диска**](ripping-a-cd.md)
</dt> </dl>

 

 





