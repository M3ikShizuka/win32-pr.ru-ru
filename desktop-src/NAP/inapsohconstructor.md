---
title: Интерфейс Инапсохконструктор (Наппротокол. h)
description: Используются SHA для создания Сохрекуестс и SHV для создания Сохреспонсес.
ms.assetid: ad79c80a-3003-4465-b350-77890c217d63
keywords:
- Инапсохконструктор интерфейса NAP
- Инапсохконструктор интерфейс NAP, описание
topic_type:
- apiref
api_name:
- INapSoHConstructor
api_location:
- qutil.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 546a6d3b4ec262fdd725af24211338e848b2b848
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065138"
---
# <a name="inapsohconstructor-interface"></a>Интерфейс Инапсохконструктор

> [!Note]  
> Платформа защиты доступа к сети недоступна начиная с Windows 10

 

**Инапсохконструктор** предоставляет методы, используемые SHA для создания [**сохрекуестс**](/windows/win32/api/naptypes/ns-naptypes-soh) и SHV для создания **сохреспонсес**.

## <a name="members"></a>Элементы

Интерфейс **инапсохконструктор** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) . **Инапсохконструктор** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **инапсохконструктор** содержит следующие методы.



| Метод                                                                                   | Описание                                         |
|:-----------------------------------------------------------------------------------------|:----------------------------------------------------|
| [**Инапсохконструктор:: Аппендаттрибуте**](inapsohconstructor-appendattribute-method.md) | Добавляет TLV в конец буфера SoH.<br/> |
| [**Инапсохконструктор:: Жетсох**](inapsohconstructor-getsoh-method.md)                   | Извлекает сконструированный пакет SoH.<br/>    |
| [**Инапсохконструктор:: Initialize**](inapsohconstructor-initialize-method.md)           | Инициализирует пакет SoH.<br/>              |
| [**Инапсохконструктор:: Validate**](inapsohconstructor-validate-method.md)               | Проверяет допустимость пакета SoH.<br/>   |



 

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

 

