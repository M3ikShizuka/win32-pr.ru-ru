---
description: Представляет коллекцию объектов EKU.
ms.assetid: 04b9f0bf-e1d4-4a2c-be5d-bae7c1090bdb
title: Объект EKU
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- EKUs
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: 56fd6eaeb5a00549cbb4ee659b99ece391e0ebed
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469924"
---
# <a name="ekus-object"></a>Объект EKU

\[CAPICOM — это 32-разрядный компонент, доступный для использования в следующих операционных системах: Windows Server 2008, Windows Vista и Windows XP. Вместо этого используйте [**класс X509ExtensionCollection**](/dotnet/api/system.security.cryptography.x509certificates.x509extensioncollection?view=netcore-3.1) в пространстве имен [**System. Security. Cryptography. X509Certificates**](/dotnet/api/system.security.cryptography.x509certificates.publickey.-ctor?view=netcore-3.1) .\]

Объект **EKU** представляет коллекцию объектов [**EKU**](eku.md) . Каждый объект [**EKU**](eku.md) представляет одно свойство расширенного использования ключа (EKU) сертификата.

## <a name="when-to-use"></a>Назначение

Коллекция **EKU** используется для выполнения следующих задач:

-   Получение числа свойств EKU в коллекции.
-   Получение определенного объекта [**EKU**](eku.md) из коллекции.
-   Выполните итерацию по коллекции.

## <a name="members"></a>Элементы

Объект **EKU** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Объект **EKU** имеет следующие свойства.



| Свойство.                                     | Тип доступа          | Описание                                                                                                                                                                                                                     |
|:---------------------------------------------|:---------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**\_NewEnum**](ekus-newenum.md)<br/> | Только для чтения<br/> | Извлекает интерфейс [**IEnumVARIANT**](/windows/win32/api/oaidl/nn-oaidl-ienumvariant) для объекта, который может быть использован для перечисления коллекции. это свойство скрыто в Visual Basic scripting Edition (VBScript).<br/> |
| [**Count**](ekus-count.md)<br/>       | Только для чтения<br/> | Возвращает число объектов [**EKU**](eku.md) в коллекции.<br/>                                                                                                                                                |
| [**Элемент**](ekus-item.md)<br/>         | Только для чтения<br/> | Извлекает объект [**EKU**](eku.md) , представляющий свойство индексированного EKU. Это свойство по умолчанию.<br/>                                                                                                      |



 

## <a name="remarks"></a>Remarks

Эта коллекция извлекается с помощью свойства [**екстендедкэйусаже. EKU**](extendedkeyusage-ekus.md) .

Не удается создать объект **EKU** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------------|----------------------------------------------------------------------------------------|
| Окончание поддержки клиента<br/> | Windows Vista<br/>                                                               |
| Поддержка конца сервера<br/> | Windows Server 2008<br/>                                                         |
| Распространяемые компоненты<br/>       | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                  |
| DLL<br/>                   | <dl> <dt>Capicom.dll</dt> </dl> |



 

 
