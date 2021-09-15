---
title: Ивмпплайлист Мовеитем, метод
description: Метод Мовеитем изменяет расположение элемента мультимедиа в списке воспроизведения.
ms.assetid: e82c820f-4640-4289-88c1-79a92e520f00
keywords:
- проигрыватель Windows Media метода мовеитем
- проигрыватель Windows Media метода мовеитем, интерфейс ивмпплайлист
- проигрыватель Windows Media интерфейса ивмпплайлист, метод мовеитем
topic_type:
- apiref
api_name:
- IWMPPlaylist.moveItem
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9c2d5be745fc3dcf799eb7203e607e493b284b4b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127459250"
---
# <a name="iwmpplaylistmoveitem-method"></a>Метод Ивмпплайлист:: Мовеитем

Метод **мовеитем** изменяет расположение элемента мультимедиа в списке воспроизведения.

## <a name="syntax"></a>Синтаксис


```CSharp
public void moveItem(
  System.Int32 lIndexOld,
  System.Int32 lIndexNew
);
```


```VB

Public Sub moveItem( _
  ByVal lIndexOld As System.Int32, _
  ByVal lIndexNew As System.Int32 _
)
Implements IWMPPlaylist.moveItem
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*линдексолд* \[ окне\]
</dt> <dd>

Объект **System. Int32** , являющийся исходным индексом.

</dd> <dt>

*линдекснев* \[ окне\]
</dt> <dd>

Объект **System. Int32** , который является новым индексом.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

Номера индексов всех элементов после вставленного элемента будут увеличены на единицу.

Перед вызовом этого метода необходимо иметь полный доступ к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                      |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ивмпплайлист (VB и C#)**](iwmpplaylist--vb-and-c.md)
</dt> <dt>

[**IWMPSettings2. Медиаакцессригхтс (VB и C#)**](wmplibiwmpsettings2-iwmpsettings2-mediaaccessrights--vb-and-c.md)
</dt> <dt>

[**IWMPSettings2. Рекуестмедиаакцессригхтс (VB и C#)**](wmplibiwmpsettings2-iwmpsettings2-requestmediaaccessrights--vb-and-c.md)
</dt> </dl>

 

 





