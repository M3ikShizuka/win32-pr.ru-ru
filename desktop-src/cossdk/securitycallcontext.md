---
description: Предоставляет доступ к контексту безопасности текущего вызова, который содержит сведения о вызывающих объектах объекта.
ms.assetid: e8ac05fb-6665-4e57-b64e-82d9799d29d4
title: Класс Секуритикаллконтекст (Комсвкс. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SecurityCallContext
api_type:
- COM
ms.openlocfilehash: bd15b7e0317a507a2340cc148bb927bb5d94a37b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570015"
---
# <a name="securitycallcontext-class"></a>Класс Секуритикаллконтекст

Предоставляет доступ к контексту безопасности текущего вызова, который содержит сведения о вызывающих объектах объекта. С помощью этого класса можно также выяснить, является ли объект прямого вызова объекта членом определенной роли и включена ли безопасность для объекта.

Только приложения COM+, использующие безопасность на основе ролей, имеют доступ к классу **секуритикаллконтекст** . Дополнительные сведения о ролях см. в разделе [Администрирование безопасности на основе ролей](role-based-security-administration.md).

## <a name="when-to-implement"></a>Когда следует реализовывать

Этот класс реализуется с помощью COM+.



| Требование | Значение |
|------------|------------------------------------------------------|
| Интерфейсы | [**исекуритикаллерсколл**](/windows/desktop/api/ComSvcs/nn-comsvcs-isecuritycallerscoll) |



 

## <a name="when-to-use"></a>Назначение

Используйте этот класс для доступа к методам [**исекуритикаллконтекст**](/windows/desktop/api/ComSvcs/nn-comsvcs-isecuritycallcontext).

## <a name="remarks"></a>Remarks

Нельзя напрямую создать объект **секуритикаллконтекст** . Чтобы использовать методы [**исекуритикаллконтекст**](/windows/desktop/api/ComSvcs/nn-comsvcs-isecuritycallcontext), необходимо получить ссылку на его реализацию, вызвав [**КОЖЕТКАЛЛКОНТЕКСТ**](/windows/desktop/api/combaseapi/nf-combaseapi-cogetcallcontext), указав IID \_ исекуритикаллконтекст для параметра *riid* .

чтобы использовать этот класс из Visual Basic майкрософт, добавьте ссылку на библиотеку типов служб COM+. Объект Секуритикаллконтекст можно объявить с помощью "Комсвкслиб. Секуритикаллконтекст" в качестве имени класса; Он создается путем вызова [**жетсекуритикаллконтекст**](/windows/desktop/api/ComSvcs/nf-comsvcs-igetsecuritycallcontext-getsecuritycallcontext).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Комсвкс. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**жетсекуритикаллконтекст**](/windows/desktop/api/ComSvcs/nf-comsvcs-igetsecuritycallcontext-getsecuritycallcontext)
</dt> <dt>

[**исекуритикаллконтекст**](/windows/desktop/api/ComSvcs/nn-comsvcs-isecuritycallcontext)
</dt> <dt>

[Безопасность программных компонентов](programmatic-component-security.md)
</dt> <dt>

[Администрирование безопасности на основе ролей](role-based-security-administration.md)
</dt> <dt>

[**секуритикаллерс**](securitycallers.md)
</dt> <dt>

[**секуритидентити**](securityidentity.md)
</dt> </dl>

 

