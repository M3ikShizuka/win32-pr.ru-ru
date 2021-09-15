---
title: Ивмпкдромбурн Бурнпрогресс, свойство
description: Свойство Бурнпрогресс возвращает ход выполнения записи компакт-диска в процентах завершения.
ms.assetid: 831cc55d-bd26-4328-a715-1a1fa48d7a40
keywords:
- проигрыватель Windows Media свойства бурнпрогресс
- проигрыватель Windows Media свойства бурнпрогресс, интерфейс ивмпкдромбурн
- проигрыватель Windows Media интерфейса ивмпкдромбурн, свойство бурнпрогресс
topic_type:
- apiref
api_name:
- IWMPCdromBurn.burnProgress
- IWMPCdromBurn.get_burnProgress
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 835c8c1091941437c226427ddb3ef53e8c577b5d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127569038"
---
# <a name="iwmpcdromburnburnprogress-property"></a>Свойство Ивмпкдромбурн:: Бурнпрогресс

Свойство **бурнпрогресс** возвращает ход выполнения записи компакт-диска в процентах завершения.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```CSharp
public System.Int32 burnProgress {get;}
```


```VB

Public ReadOnly Property burnProgress As System.Int32
```





## <a name="property-value"></a>Значение свойства

Значение **System. Int32** , которое является значением хода выполнения. Значения хода выполнения находятся в диапазоне от 0 до 100.

## <a name="remarks"></a>Remarks

Значение Progress представляет завершенный процент всего процесса записи, включая все промежуточные операции.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 11<br/>                                                                                     |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ивмпкдромбурн (VB и C#)**](iwmpcdromburn--vb-and-c.md)
</dt> </dl>

 

 





