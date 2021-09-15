---
title: Ивмпкдромбурн, свойство метки
description: Свойство Label получает строку метки тома компакт-диска.
ms.assetid: 46e7741c-59c5-46d8-b9ca-09892d907cd7
keywords:
- проигрыватель Windows Media свойства метки
- свойство метки проигрыватель Windows Media, интерфейс ивмпкдромбурн
- проигрыватель Windows Media интерфейса ивмпкдромбурн, свойство label
topic_type:
- apiref
api_name:
- IWMPCdromBurn.label
- IWMPCdromBurn.get_label
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 05da344f1148de7e79cb605135964c6ab8225ac0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127569014"
---
# <a name="iwmpcdromburnlabel-property"></a>Ивмпкдромбурн:: Label, свойство

Свойство *Label* получает строку метки тома компакт-диска.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```CSharp
public System.String label {get;}
```


```VB

Public ReadOnly Property label As System.String
```





## <a name="property-value"></a>Значение свойства

Строка **System. String** , которая является строкой метки тома.

## <a name="remarks"></a>Remarks

В связи с тем, как хранятся метки компакт-дисков, метка компакт-диска может быть короче длины указанной строки метки тома. Если длина строки превышает максимальную длину метки компакт-диска, текст будет обрезан.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 11.<br/>                                                                                    |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ивмпкдромбурн (VB и C#)**](iwmpcdromburn--vb-and-c.md)
</dt> </dl>

 

 





