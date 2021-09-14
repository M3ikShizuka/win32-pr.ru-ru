---
title: IWMPMedia3 Жетаттрибутекаунтбитипе, метод
description: Метод Жетаттрибутекаунтбитипе возвращает число атрибутов, связанных с указанным типом атрибута.
ms.assetid: d692635f-f9f1-4d8e-a9c5-9d7fa84f41bd
keywords:
- проигрыватель Windows Media метода жетаттрибутекаунтбитипе
- проигрыватель Windows Media метода жетаттрибутекаунтбитипе, интерфейс IWMPMedia3
- проигрыватель Windows Media интерфейса IWMPMedia3, метод жетаттрибутекаунтбитипе
topic_type:
- apiref
api_name:
- IWMPMedia3.getAttributeCountByType
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 49505f9e9df8778cc2c17ba062da6700b9b8aec4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172719"
---
# <a name="iwmpmedia3getattributecountbytype-method"></a>Метод IWMPMedia3:: Жетаттрибутекаунтбитипе

Метод **жетаттрибутекаунтбитипе** возвращает число атрибутов, связанных с указанным типом атрибута.

## <a name="syntax"></a>Синтаксис


```CSharp
public System.Int32 getAttributeCountByType(
  System.String bstrType,
  System.String bstrLanguage
);
```


```VB

Public Function getAttributeCountByType( _
  ByVal bstrType As System.String, _
  ByVal bstrLanguage As System.String _
) As System.Int32
Implements IWMPMedia3.getAttributeCountByType
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*бстртипе* \[ окне\]
</dt> <dd>

**Строка System. String** , которая является типом атрибута.

</dd> <dt>

*бстрлангуаже* \[ окне\]
</dt> <dd>

**Строка System. String** , которая является языком. Если задано значение null или строка нулевой длины (""), используется текущая строка языкового стандарта. В противном случае значение должно быть допустимой строкой языка RFC 1766, например "en-US".

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Объект **System. Int32** , который является количеством атрибутов, связанных с типом.

## <a name="remarks"></a>Remarks

Этот метод используется для определения количества атрибутов, соответствующих определенному имени атрибута для данного элемента мультимедиа. Номера индексов можно передать в метод **жетитеминфобитипе** . Это полезно, например, когда элемент мультимедиа был разбит на несколько жанров.

Перед вызовом этого метода необходимо иметь доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                      |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс IWMPMedia3 (VB и C#)**](iwmpmedia3--vb-and-c.md)
</dt> <dt>

[**IWMPMedia3. Жетитеминфобитипе (VB и C#)**](wmplibiwmpmedia3-iwmpmedia3-getiteminfobytype--vb-and-c.md)
</dt> </dl>

 

 





