---
title: Метод шага IWMPControls2
description: Метод Step заставляет текущий элемент мультимедиа перейти к следующему кадру или предыдущему кадру и заморозить воспроизведение.
ms.assetid: c5cb720f-527f-45b6-ae8a-4da0e3e34618
keywords:
- проигрыватель Windows Media метода step
- проигрыватель Windows Media метода step, интерфейс IWMPControls2
- проигрыватель Windows Media интерфейса IWMPControls2, метод step
topic_type:
- apiref
api_name:
- IWMPControls2.step
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4cfb65dd20de506a8f303121b23668e2fbf14dc4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064209"
---
# <a name="iwmpcontrols2step-method"></a>Метод IWMPControls2:: Step

Метод **Step** заставляет текущий элемент мультимедиа перейти к следующему кадру или предыдущему кадру и заморозить воспроизведение.

## <a name="syntax"></a>Синтаксис


```CSharp
public void step(
  System.Int32 lStep
);
```


```VB

Public Sub step( _
  ByVal lStep As System.Int32 _
)
Implements IWMPControls2.step
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*лстеп* \[ окне\]
</dt> <dd>

Значение **System. Int32** , указывающее, сколько кадров необходимо выполнить перед замораживанием. Необходимо задать значение 1 или-1.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

В настоящее время этот метод поддерживает только параметры 1 или-1, поэтому можно пошаговым образом выполнять только один кадр.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                      |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс IWMPControls2 (VB и C#)**](iwmpcontrols2--vb-and-c.md)
</dt> <dt>

[**Интерфейс ИВМПДВД (VB и C#)**](iwmpdvd--vb-and-c.md)
</dt> </dl>

 

 





