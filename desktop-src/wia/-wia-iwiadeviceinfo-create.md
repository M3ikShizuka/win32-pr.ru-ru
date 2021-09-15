---
description: метод Create объекта DeviceInfo устанавливает соединение с устройством Windowsного получения изображений (WIA), заданным объектом DeviceInfo, и возвращает объект Item, представляющий устройство.
ms.assetid: 57f3698c-3f9f-4775-8b53-a65a5591aa3d
title: DeviceInfo. Create, метод
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DeviceInfo.Create
api_type:
- COM
api_location:
- Wiascr.dll
ms.openlocfilehash: 1efc36ea8794de4b64c9af616320b09d547f6490
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127571378"
---
# <a name="deviceinfocreate-method"></a>DeviceInfo. Create, метод

метод **Create** объекта [**DeviceInfo**](-wia-deviceinfo.md) устанавливает соединение с устройством Windowsного получения изображений (WIA), заданным объектом **DeviceInfo** , и возвращает объект [**Item**](-wia-item.md) , представляющий устройство.

## <a name="syntax"></a>Синтаксис


```JScript
retVal = DeviceInfo.Create()
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Тип: **ивиадиспатчитем**

Этот метод возвращает объект [**Item**](-wia-item.md) , представляющий созданное устройство.

## <a name="remarks"></a>Remarks

Используйте метод **CREATE** , чтобы создать подключение к аппаратному устройству WIA после перечисления коллекции [**устройств**](-wia-iwia-devices.md) . Метод возвращает объект [**Item**](-wia-item.md) , представляющий устройство (корневой элемент).

## <a name="examples"></a>Примеры

В следующем примере демонстрируется использование метода **CREATE** .


```JScript
<SCRIPT LANGUAGE="VBScript">
Dim objWia
Dim objDeviceInfoCollection
Dim objDeviceInfo
Dim objItem
 
Set objWIA = CreateObject("Wia.Script")
 
Set objDeviceInfoCollection = objWia.Devices
 
For Each objDeviceInfo In objDeviceInfoCollection
    Set objItem = objDeviceInfo.Create()
Next
</SCRIPT>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional, только для \[ настольных приложений Windows XP\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                          |
| DLL<br/>                      | <dl> <dt>Wiascr.dll (версия 4,90 или более поздняя)</dt> </dl> |



 

 




