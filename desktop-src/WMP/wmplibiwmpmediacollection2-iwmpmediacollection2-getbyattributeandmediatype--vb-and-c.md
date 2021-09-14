---
title: IWMPMediaCollection2 Жетбяттрибутеандмедиатипе, метод
description: Метод Жетбяттрибутеандмедиатипе возвращает интерфейс Ивмпплайлист, предоставляющий доступ к элементам мультимедиа с указанным атрибутом и типом мультимедиа.
ms.assetid: dce9cef4-1d12-4bee-a75d-42274556c5bc
keywords:
- проигрыватель Windows Media метода жетбяттрибутеандмедиатипе
- проигрыватель Windows Media метода жетбяттрибутеандмедиатипе, интерфейс IWMPMediaCollection2
- проигрыватель Windows Media интерфейса IWMPMediaCollection2, метод жетбяттрибутеандмедиатипе
topic_type:
- apiref
api_name:
- IWMPMediaCollection2.getByAttributeAndMediaType
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: fb1ee4e9421b4546cdc8ace6173dacab5034b905
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127342767"
---
# <a name="iwmpmediacollection2getbyattributeandmediatype-method"></a>Метод IWMPMediaCollection2:: Жетбяттрибутеандмедиатипе

`getByAttributeAndMediaType`Метод возвращает интерфейс **ивмпплайлист** , предоставляющий доступ к элементам мультимедиа с указанным атрибутом и типом мультимедиа.

## <a name="syntax"></a>Синтаксис


```CSharp
public IWMPPlaylist getByAttributeAndMediaType(
  System.String bstrAttribute,
  System.String bstrValue,
  System.String bstrMediaType
);
```


```VB

Public Function getByAttributeAndMediaType( _
  ByVal bstrAttribute As System.String, _
  ByVal bstrValue As System.String, _
  ByVal bstrMediaType As System.String _
) As IWMPPlaylist
Implements IWMPMediaCollection2.getByAttributeAndMediaType
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*бстраттрибуте* \[ окне\]
</dt> <dd>

**Строка System. String** , которая является указанным атрибутом.

</dd> <dt>

*бстрвалуе* \[ окне\]
</dt> <dd>

**Строка System. String** , которая является заданным значением для атрибута, указанного в *бстраттрибуте*.

</dd> <dt>

*бстрмедиатипе* \[ окне\]
</dt> <dd>

**Строка System. String** , которая является указанным типом носителя.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Интерфейс **вмплиб. ивмпплайлист** для полученного списка воспроизведения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 11.<br/>                                                                                    |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс IWMPMediaCollection2 (VB и C#)**](iwmpmediacollection2--vb-and-c.md)
</dt> <dt>

[**Интерфейс Ивмпплайлист (VB и C#)**](iwmpplaylist--vb-and-c.md)
</dt> </dl>

 

 





