---
title: Ивмпкдромколлектион Count, свойство
description: Свойство Count получает количество доступных компакт-дисков и DVD-дисководов в системе.
ms.assetid: 1359ab7e-fbe3-461c-801b-7c986f6e5687
keywords:
- проигрыватель Windows Media свойства count
- свойство count проигрыватель Windows Media, интерфейс ивмпкдромколлектион
- интерфейс ивмпкдромколлектион проигрыватель Windows Media, свойство count
topic_type:
- apiref
api_name:
- IWMPCdromCollection.count
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a2da4d4d443c730d19c791a486fed4be0241b8c5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127569002"
---
# <a name="iwmpcdromcollectioncount-property"></a>Свойство Ивмпкдромколлектион:: count

Свойство **Count** получает количество доступных компакт-дисков и DVD-дисководов в системе.

## <a name="syntax"></a>Синтаксис


```CSharp
public System.Int32 count {get; set;}
```


```VB

Public ReadOnly Property count As System.Int32
```





## <a name="property-value"></a>Значение свойства

Значение **System. Int32** , которое является счетчиком доступных дисков.

## <a name="remarks"></a>Remarks

Чтобы получить значение этого свойства, требуется доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

Диски DVD подсчитываются точно так же, как и дисководы компакт-дисков. однако элемент управления проигрыватель Windows Media ActiveX поддерживает только функции DVD для Windows XP и более поздних версий. Обычно дисководы DVD могут воспроизводить компакт-диски, но дисководы компакт-дисков не могут воспроизводить DVD-носители.

## <a name="examples"></a>Примеры

В следующем примере функция Count используется для вывода в окне сообщения числа доступных дисководов компакт-дисков и DVD. Объект Аксвмплиб. Аксвиндовсмедиаплайер представлен переменной с именем Player.


```CSharp
// Store the number of available drives.
int numDrives = player.cdromCollection.count;

// Display the number of drives as a string.
System.Windows.Forms.MessageBox.Show("Number of available CD and DVD drives:  " + numDrives.ToString());
```


```VB

' Store the number of available drives.
Dim numDrives As Integer = player.cdromCollection.count

&#39; Display the number of drives as a string.
System.Windows.Forms.MessageBox.Show(&quot;Number of available CD and DVD drives:  &quot; + numDrives.ToString())
```





## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                      |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ивмпкдромколлектион (VB и C#)**](iwmpcdromcollection--vb-and-c.md)
</dt> <dt>

[**IWMPSettings2. Медиаакцессригхтс (VB и C#)**](wmplibiwmpsettings2-iwmpsettings2-mediaaccessrights--vb-and-c.md)
</dt> <dt>

[**IWMPSettings2. Рекуестмедиаакцессригхтс (VB и C#)**](wmplibiwmpsettings2-iwmpsettings2-requestmediaaccessrights--vb-and-c.md)
</dt> </dl>

 

 





