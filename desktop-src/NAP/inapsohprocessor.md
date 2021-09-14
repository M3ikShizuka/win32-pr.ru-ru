---
title: Интерфейс Инапсохпроцессор (Наппротокол. h)
description: Используются SHA для обработки содержимого Сохреспонсес и SHV для обработки содержимого Сохрекуестс.
ms.assetid: c2dd71ca-a4dd-44d2-81ab-b83e90599a2f
keywords:
- Инапсохпроцессор интерфейса NAP
- Инапсохпроцессор интерфейс NAP, описание
topic_type:
- apiref
api_name:
- INapSoHProcessor
api_location:
- qutil.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1c43abf137bb267468deeb9d4bd47546275ba6c7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065125"
---
# <a name="inapsohprocessor-interface"></a>Интерфейс Инапсохпроцессор

> [!Note]  
> Платформа защиты доступа к сети недоступна начиная с Windows 10

 

**Инапсохпроцессор** предоставляет методы, используемые SHA для обработки содержимого [**сохреспонсес**](/windows/win32/api/naptypes/ns-naptypes-soh) и SHV для обработки содержимого **сохрекуестс**.

## <a name="members"></a>Элементы

Интерфейс **инапсохпроцессор** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) . **Инапсохпроцессор** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **инапсохпроцессор** содержит следующие методы.



| Метод                                                                                           | Описание                                                                           |
|:-------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------|
| [**Инапсохпроцессор:: Финднекстаттрибуте**](inapsohprocessor-findnextattribute-method.md)         | Находит индекс расположения следующего атрибута пакета SoH.<br/>                 |
| [**Инапсохпроцессор:: OutAttribute**](inapsohprocessor-getattribute-method.md)                   | Извлекает тип и значение атрибута.<br/>                                    |
| [**Инапсохпроцессор:: Жетнумберофаттрибутес**](inapsohprocessor-getnumberofattributes-method.md) | Извлекает количество атрибутов, содержащихся в SoH.<br/>                   |
| [**Инапсохпроцессор:: Initialize**](inapsohprocessor-initialize-method.md)                       | Инициализирует пакет протокола SoH и систему защиты доступа к сети для обработки содержимого.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                       |
| Заголовок<br/>                   | <dl> <dt>Наппротокол. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Наппротокол. idl</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Qutil.dll</dt> </dl>       |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Интерфейсы NAP](nap-interfaces.md)
</dt> <dt>

[Справочник по NAP](nap-reference.md)
</dt> </dl>

 

