---
description: Свойство Компоненткуррентстате объекта Session является свойством только для чтения, которое возвращает текущее установленное состояние указанного компонента. Значения состояния см. в описании свойства Компонентрекуестстате.
ms.assetid: c8343e90-8867-462d-9844-e547341a590c
title: Свойство Session. Компоненткуррентстате
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Session.ComponentCurrentState
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 8c556dd9656ebced155ef90fe96abd394a32ff1b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055279"
---
# <a name="sessioncomponentcurrentstate-property"></a>Свойство Session. Компоненткуррентстате

Свойство **компоненткуррентстате** объекта [**Session**](session-object.md) является свойством только для чтения, которое возвращает текущее установленное состояние указанного компонента. Значения состояния см. в описании свойства [**компонентрекуестстате**](session-componentrequeststate.md) .

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Session.ComponentCurrentState
```



## <a name="property-value"></a>Значение свойства

Требуемое строковое имя запрошенного компонента, первичный ключ в таблице Component.

## <a name="remarks"></a>Комментарии

Если свойство завершается неудачно, можно получить расширенные сведения об ошибке с помощью метода [**ластерроррекорд**](installer-lasterrorrecord.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ ISession определяется как 000C109E-0000-0000-C000-000000000046<br/>                                                                                                                                                                             |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Сеанс**](session-object.md)
</dt> <dt>

[**Компонентрекуестстате, свойство**](session-componentrequeststate.md)
</dt> </dl>

 

 




