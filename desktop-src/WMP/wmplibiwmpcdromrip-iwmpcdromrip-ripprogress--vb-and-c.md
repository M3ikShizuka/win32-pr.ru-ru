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
ms.openlocfilehash: 113b9fc716698156aa4f7731a7b19888e0edf438
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127568994"
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

## <a name="requirements"></a>Требования



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

 

 





