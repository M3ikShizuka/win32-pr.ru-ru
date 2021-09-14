---
title: Ивмпклоседкаптион Каптионингид, свойство
description: Свойство Ивмпклоседкаптион Возвращает или задает имя HTML-элемента, отображающего субтитры.
ms.assetid: b09bb7c7-c3b6-4e0d-962f-24b06a04f6d1
keywords:
- проигрыватель Windows Media свойства каптионингид
- проигрыватель Windows Media свойства каптионингид, интерфейс ивмпклоседкаптион
- проигрыватель Windows Media интерфейса ивмпклоседкаптион, свойство каптионингид
topic_type:
- apiref
api_name:
- IWMPClosedCaption.captioningId
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 343234fce2b93ac02255731a38025f6d7b9fac6f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127242980"
---
# <a name="iwmpclosedcaptioncaptioningid-property"></a>Свойство Ивмпклоседкаптион:: Каптионингид

Свойство **ивмпклоседкаптион** Возвращает или задает имя HTML-элемента, отображающего субтитры.

## <a name="syntax"></a>Синтаксис


```CSharp
public System.String captioningId {get; set;}
```


```VB

Public Property captioningId As System.String
```





## <a name="property-value"></a>Значение свойства

**Строка System. String** , которая является идентификатором HTML-элемента.

## <a name="remarks"></a>Remarks

Указанное имя элемента может быть любым HTML-элементом на веб-странице, если он поддерживает атрибут **InnerHtml** . если веб-страница содержит несколько кадров, имя элемента может ссылаться только на элемент в том же кадре, что и элемент управления проигрыватель Windows Media.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                      |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Добавление субтитров к цифровым носителям**](adding-closed-captions-to-digital-media.md)
</dt> <dt>

[**Интерфейс Ивмпклоседкаптион (VB и C#)**](iwmpclosedcaption--vb-and-c.md)
</dt> <dt>

[**Интерфейс IWMPClosedCaption2 (VB и C#)**](iwmpclosedcaption2--vb-and-c.md)
</dt> </dl>

 

 





