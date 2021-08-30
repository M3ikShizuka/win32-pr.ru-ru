---
description: Содержит методы, позволяющие получать доступ и изменять параметры безопасности для пространства имен.
ms.assetid: a54fdd85-feb8-4727-9f26-fe4f213cab6b
ms.tgt_platform: multiple
title: Класс __SystemSecurity
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- __SystemSecurity
api_type:
- Schema
api_location:
- All
ms.openlocfilehash: 141e659c0ddf15c0369323e5d18d6251c3334a47
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122468531"
---
# <a name="__systemsecurity-class"></a>\_\_Класс Системсекурити

Класс System **\_ \_ системсекурити** содержит методы, позволяющие получать доступ к параметрам безопасности пространства имен и изменять их. Класс **\_ \_ системсекурити** является Singleton-классом в каждом пространстве имен.

> [!Note]  
> Дополнительные сведения см. в разделе [Настройка дескрипторов безопасности намепаце](setting-namespace-security-descriptors.md).

 

Приведенный ниже синтаксис является упрощенной версией кода MOF и включает все унаследованные свойства. Свойства перечислены в алфавитном порядке, а не в MOF.

## <a name="syntax"></a>Синтаксис

``` syntax
class __SystemSecurity
{
};
```

## <a name="members"></a>Члены

Класс **\_ \_ системсекурити** имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Класс **\_ \_ системсекурити** содержит следующие методы.




| Метод | Описание | 
|--------|-------------|
| <a href="--systemsecurity-get9xuserlist.md"><strong>Get9XUserList</strong></a> | Возвращает список пользователей, которым разрешен удаленный доступ.<br /><blockquote>[!Note]<br />Этот метод не работает в поддерживаемых версиях Windows. Вместо этого используйте <a href="--systemsecurity-getsd.md"><strong>возвращает</strong></a> .</blockquote><br /> | 
| <a href="--systemsecurity-getcalleraccessrights.md"><strong>жеткаллеракцессригхтс</strong></a> | Возвращает маску для каждого бита, соответствующего право доступа.<br /> | 
| <a href="--systemsecurity-getsd.md"><strong>Получает</strong></a> | Возвращает <a href="/windows/desktop/api/winnt/ns-winnt-security_descriptor"><strong>SECURITY_DESCRIPTOR</strong></a> для пространства имен, к которому подключен пользователь.<br /> | 
| <a href="getsecuritydescriptor-method-in-class---systemsecurity-.md"><strong>жетсекуритидескриптор</strong></a> | Возвращает дескриптор безопасности, управляющий доступом к пространству имен WMI, связанному с экземпляром <strong>__SystemSecurity</strong>. Дескриптор безопасности возвращается как экземпляр<a href="--securitydescriptor.md"><strong>__SecurityDescriptor</strong></a>.<br /> | 
| <a href="--systemsecurity-set9xuserlist.md"><strong>Set9XUserList</strong></a> | Задает список пользователей, которым разрешен удаленный доступ.<br /><blockquote>[!Note]<br />Этот метод не работает в поддерживаемых версиях Windows. Вместо этого используйте <a href="--systemsecurity-setsd.md"><strong>набор</strong></a> .</blockquote><br /> | 
| <a href="--systemsecurity-setsd.md"><strong>Устанавливается</strong></a> | Задает дескриптор безопасности для пространства имен, к которому подключен пользователь.<br /> | 
| <a href="setsecuritydescriptor-method-in-class---systemsecurity.md"><strong>сетсекуритидескриптор</strong></a> | Записывает обновленную версию дескриптора безопасности, которая управляет доступом к принтеру. Дескриптор безопасности представлен экземпляром <a href="--securitydescriptor.md"><strong>__SecurityDescriptor</strong></a>.<br /> | 




 

## <a name="remarks"></a>Комментарии

Можно потребовать, чтобы клиентские скрипты и приложения использовали зашифрованное соединение для проверки подлинности, добавив квалификатор **рекуиресенкриптион** в MOF-файл, который создает пространство имен. Можно также изменить существующее пространство имен, добавив этот атрибут и повторно скомпилировать MOF-файл. Дополнительные сведения об использовании **рекуиресенкриптион** см. в разделе [запрос зашифрованного соединения с пространством имен](requiring-an-encrypted-connection-to-a-namespace.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>       |
| Минимальная версия сервера<br/> | Windows Server 2008<br/> |
| Пространство имен<br/>                | Все пространства имен WMI<br/>  |



## <a name="see-also"></a>См. также

<dl> <dt>

[Системные классы WMI](wmi-system-classes.md)
</dt> <dt>

[Константы безопасности WMI](wmi-security-constants.md)
</dt> <dt>

[Объекты дескрипторов безопасности WMI](wmi-security-descriptor-objects.md)
</dt> <dt>

[Защита пространств имен WMI](securing-wmi-namespaces.md)
</dt> <dt>

[Установка наследования безопасности пространства имен](establishing-inheritance-of-namespace-security.md)
</dt> <dt>

[Списки управления доступом (ACL)](/windows/desktop/SecAuthZ/access-control-lists)
</dt> <dt>

[**\_Дескриптор безопасности**](/windows/desktop/api/winnt/ns-winnt-security_descriptor)
</dt> </dl>

