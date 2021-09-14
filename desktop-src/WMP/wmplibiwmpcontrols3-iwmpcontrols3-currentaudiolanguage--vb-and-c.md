---
title: IWMPControls3 Куррентаудиолангуаже, свойство
description: Свойство Куррентаудиолангуаже Возвращает или задает код локали (LCID) звукового языка для воспроизведения.
ms.assetid: 4adf26c7-077a-483e-8a76-accf871eca4c
keywords:
- проигрыватель Windows Media свойства куррентаудиолангуаже
- проигрыватель Windows Media свойства куррентаудиолангуаже, интерфейс IWMPControls3
- проигрыватель Windows Media интерфейса IWMPControls3, свойство куррентаудиолангуаже
topic_type:
- apiref
api_name:
- IWMPControls3.currentAudioLanguage
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7c4621b5eace56cb883a6c8b14c3b1f082b12d3a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064207"
---
# <a name="iwmpcontrols3currentaudiolanguage-property"></a>Свойство IWMPControls3:: Куррентаудиолангуаже

Свойство **куррентаудиолангуаже** Возвращает или задает код локали (LCID) звукового языка для воспроизведения.

## <a name="syntax"></a>Синтаксис


```CSharp
public System.Int32 currentAudioLanguage {get; set;}
```


```VB

Public Property currentAudioLanguage As System.Int32
```





## <a name="property-value"></a>Значение свойства

Объект **System. Int32** , который является идентификатором языка аудио.

## <a name="remarks"></a>Remarks

Код языка (LCID) однозначно определяет определенный диалект языка, который называется локальным языком.

для Windows содержимого на основе носителя свойства и методы, связанные с выбором языка, поддерживают только один выход.

При работе с содержимым DVD при указании LCID будет выбрана первая доступная звуковая дорожка с указанным ИДЕНТИФИКАТОРом языка.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                      |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс IWMPControls3 (VB и C#)**](iwmpcontrols3--vb-and-c.md)
</dt> <dt>

[**IWMPControls3. Аудиолангуажекаунт (VB и C#)**](wmplibiwmpcontrols3-iwmpcontrols3-audiolanguagecount--vb-and-c.md)
</dt> <dt>

[**IWMPControls3. Куррентаудиолангуажеиндекс (VB и C#)**](wmplibiwmpcontrols3-iwmpcontrols3-currentaudiolanguageindex--vb-and-c.md)
</dt> <dt>

[**IWMPControls3. Жетаудиолангуажедескриптион (VB и C#)**](wmplibiwmpcontrols3-iwmpcontrols3-getaudiolanguagedescription--vb-and-c.md)
</dt> <dt>

[**IWMPControls3. Жетаудиолангуажеид (VB и C#)**](wmplibiwmpcontrols3-iwmpcontrols3-getaudiolanguageid--vb-and-c.md)
</dt> <dt>

[**IWMPControls3. Жетлангуаженаме (VB и C#)**](wmplibiwmpcontrols3-iwmpcontrols3-getlanguagename--vb-and-c.md)
</dt> </dl>

 

 





