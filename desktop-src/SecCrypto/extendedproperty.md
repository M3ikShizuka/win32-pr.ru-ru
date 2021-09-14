---
description: Представляет свойство, расширенное корпорацией Майкрософт.
ms.assetid: 91375fd5-b3af-4ed4-961d-5cc1db1a14e3
title: Объект ExtendedProperty
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ExtendedProperty
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: 2ec61da301dc1819c899a7da23da9a10efd81ae0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171039"
---
# <a name="extendedproperty-object"></a>Объект ExtendedProperty

\[CAPICOM — это 32-разрядный компонент, доступный для использования в следующих операционных системах: Windows Server 2008, Windows Vista и Windows XP. Вместо этого используйте службы вызова платформы (PInvoke) для вызова функции Win32 API [**цертжетцертификатеконтекстпроперти**](/windows/desktop/api/Wincrypt/nf-wincrypt-certgetcertificatecontextproperty) и получения свойств. Дополнительные сведения о PInvoke см. в разделе [учебник по вызову неуправляемого](https://msdn.microsoft.com/library/aa288468.aspx)кода. [.NET и CryptoAPI через p/Invoke: часть 1](/previous-versions/ms867087(v=msdn.10)#netcryptoapi_topic5) и [.NET и CryptoAPI через p/Invoke: часть 2](/previous-versions/ms867087(v=msdn.10)#netcryptoapi_topic6) подразделы [расширения шифрования .NET с помощью CAPICOM и P/Invoke](/previous-versions/ms867087(v=msdn.10)) также могут быть полезными.\]

Объект **ExtendedProperty** представляет свойство, расширенное корпорацией Майкрософт.

## <a name="when-to-use"></a>Назначение

Объект **ExtendedProperty** используется для выполнения следующих задач:

-   Задайте или получите тип расширенного свойства.
-   Установка или получение типа кодировки, используемой для кодирования расширенного свойства.

## <a name="members"></a>Элементы

Объект **ExtendedProperty** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Объект **ExtendedProperty** имеет следующие свойства.



| Свойство                                             | Тип доступа           | Описание                                                                                                                                                                    |
|:-----------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**PropID**](extendedproperty-propid.md)<br/> | Чтение/запись<br/> | Значение перечисления [**CAPICOM \_ PropID**](capicom-propid.md) , которое задает или получает тип расширенного свойства.<br/> Это свойство по умолчанию.<br/> |
| [**Значение**](extendedproperty-value.md)<br/>   | Чтение/запись<br/> | Значение перечисления [**\_ \_ типа CAPICOM Encoding**](capicom-encoding-type.md) , которое задает или получает данные расширенного свойства.<br/>                              |



 

## <a name="remarks"></a>Комментарии

Объект **ExtendedProperty** используется коллекцией [**расширенных свойств**](extendedproperties.md) .

Объект **ExtendedProperty** может быть создан и не является надежным для скриптов. ProgID для объекта **ExtendedProperty** — CAPICOM. ExtendedProperty. 1.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------------|----------------------------------------------------------------------------------------|
| Окончание поддержки клиента<br/> | Windows Vista<br/>                                                               |
| Поддержка конца сервера<br/> | Windows Server 2008<br/>                                                         |
| Распространяемые компоненты<br/>       | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                  |
| DLL<br/>                   | <dl> <dt>Capicom.dll</dt> </dl> |



 

 
