---
description: Задает или получает значение общего свойства.
ms.assetid: 19ed8d50-3ac1-408e-9f25-09f284d025f1
title: Класс Шаредпроперти (Комсвкс. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SharedProperty
api_type:
- COM
ms.openlocfilehash: a7a7857ad280ad722601bdced6c25d04b03dc0b3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127347575"
---
# <a name="sharedproperty-class"></a>Класс Шаредпроперти

Задает или получает значение общего свойства.

Общие сведения об использовании общего диспетчер свойств в COM+ см. в разделе [com+ shared Диспетчер свойств](com--shared-property-manager.md).

## <a name="when-to-implement"></a>Когда следует реализовывать

Этот класс реализуется с помощью COM+.



| Требование | Значение |
|------------|--------------------------------------------|
| Интерфейсы | [**ишаредпроперти**](/windows/desktop/api/ComSvcs/nn-comsvcs-isharedproperty) |



 

## <a name="when-to-use"></a>Назначение

Используйте этот класс для доступа к методам [**ишаредпроперти**](/windows/desktop/api/ComSvcs/nn-comsvcs-isharedproperty).

## <a name="remarks"></a>Remarks

Объект **шаредпроперти** можно создать с помощью методов [**CreateProperty**](/windows/desktop/api/ComSvcs/nf-comsvcs-isharedpropertygroup-createproperty) или [**креатепропертибипоситион**](/windows/desktop/api/ComSvcs/nf-comsvcs-isharedpropertygroup-createpropertybyposition) [**ишаредпропертиграуп**](/windows/desktop/api/ComSvcs/nn-comsvcs-isharedpropertygroup).

чтобы использовать этот класс из Visual Basic майкрософт, добавьте ссылку на библиотеку типов служб COM+. Объект Шаредпроперти создается путем вызова методов [**CreateProperty**](/windows/desktop/api/ComSvcs/nf-comsvcs-isharedpropertygroup-createproperty) или [**креатепропертибипоситион**](/windows/desktop/api/ComSvcs/nf-comsvcs-isharedpropertygroup-createpropertybyposition) объекта [**шаредпропертиграуп**](sharedpropertygroup.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Комсвкс. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ишаредпроперти**](/windows/desktop/api/ComSvcs/nn-comsvcs-isharedproperty)
</dt> <dt>

[**шаредпропертиграуп**](sharedpropertygroup.md)
</dt> <dt>

[**шаредпропертиграупманажер**](sharedpropertygroupmanager.md)
</dt> </dl>

 

 




