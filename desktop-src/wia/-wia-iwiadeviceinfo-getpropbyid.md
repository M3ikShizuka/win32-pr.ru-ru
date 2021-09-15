---
description: Метод Жетпропбид объекта DeviceInfo использует идентификатор свойства устройства для возвращения его значения.
ms.assetid: 9c68e6af-446c-4750-89e6-70862b23b296
title: DeviceInfo. Жетпропбид, метод
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DeviceInfo.GetPropById
api_type:
- COM
api_location:
- Wiascr.dll
ms.openlocfilehash: adbc8b6a29f97066c8dc5b2e45b7ddc5834f2b60
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127571374"
---
# <a name="deviceinfogetpropbyid-method"></a>DeviceInfo. Жетпропбид, метод

Метод **жетпропбид** объекта [**DeviceInfo**](-wia-deviceinfo.md) использует идентификатор свойства устройства для возвращения его значения.

## <a name="syntax"></a>Синтаксис


```JScript
retVal = DeviceInfo.GetPropById(
  Id
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Идентификатор* \[ в\]
</dt> <dd>

Тип: **[виадевицеинфопропертид](-wia-wiadeviceinfopropertyid.md)**

Указывает идентификатор свойства.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **Variant**

Этот метод возвращает значение свойства, заданного *идентификатором*.

## <a name="remarks"></a>Remarks

Используйте этот метод, чтобы найти значение свойства устройства по его ИДЕНТИФИКАТОРу. Список идентификаторов свойств см. в разделе [определения констант свойств WIA](-wia-wia-property-constant-definitions.md). сведения о самих свойствах Windowsного получения изображений (wia) см. в разделе [константы свойства wia](-wia-wia-property-constants.md).

для приложений Microsoft Visual Basic добавьте ссылку на "Windows получения образа библиотеки типов 1,01". Следующие константы, определенные в этом файле, допустимы для этого метода:

``` syntax
const DeviceID = 2
const Manufacturer = 3
const Description = 4
const Type = 5
const Port = 6
const Name = 7
const Server = 8
const RemoteDevID = 9
const UIClassID = 10
```

## <a name="examples"></a>Примеры

В следующем примере демонстрируется использование метода **жетпропбид** для получения значения свойства.


```JScript
<SCRIPT LANGUAGE="VBScript">
const WIA_DIP_DEV_TYPE = 5
Dim objWia
Dim objDeviceInfoCollection
Dim objDeviceInfo
Dim PropValue
 
Set objWIA = CreateObject("Wia.Script")
 
Set objDeviceInfoCollection = objWia.Devices
 
For Each objDeviceInfo In objDeviceInfoCollection
    PropValue = objDeviceInfo.GetPropById(WIA_DIP_DEV_TYPE)
Next
</SCRIPT>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional, только для \[ настольных приложений Windows XP\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                          |
| DLL<br/>                      | <dl> <dt>Wiascr.dll (версия 4,90 или более поздняя)</dt> </dl> |



 

 




