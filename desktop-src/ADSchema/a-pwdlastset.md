---
title: PWD-Last-Set, атрибут
description: Дата и время последнего изменения пароля для этой учетной записи.
ms.assetid: 06ca5cd5-a285-488a-9db0-c698b82a847d
ms.tgt_platform: multiple
keywords:
- PWD-Last-Set схема AD атрибута
- Схема AD атрибута pwdLastSet
topic_type:
- apiref
api_name:
- Pwd-Last-Set
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a43c4ca87523e94c69d575495339d5491b1d650d059fbf2b7ab9a046cad98275
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119837514"
---
# <a name="pwd-last-set-attribute"></a>PWD-Last-Set, атрибут

Дата и время последнего изменения пароля для этой учетной записи. Это значение хранится в виде большого целого числа, представляющего количество интервалов в 100 нс, начиная с 1 января 1601 (UTC). Если это значение равно 0, а атрибут [**User-Account-Control**](a-useraccountcontrol.md) не содержит флаг **УФ \_ не \_ Expires \_ PASSWD** , то пользователь должен задать пароль при следующем входе в систему.



| Ввод | Значение |
|-------------------|--------------------------------------|
| CN                | PWD-Last-Set                         |
| LDAP-отображаемое имя | pwdLastSet                           |
| Размер              | 8 байт                              |
| Привилегия обновления  | Это значение задается системой.     |
| Частота обновления  | При каждом изменении пароля.   |
| Attribute-Id      | 1.2.840.113556.1.4.96                |
| System-ID — GUID    | bf967a0a-0de6-11d0-a285-00aa003049e2 |
| Синтаксис            | [**Интервал**](s-interval.md)       |



## <a name="implementations"></a>Варианты реализации решения

-   [**Windows 2000 Server**](#windows-2000-server)
-   [**Windows Server 2003**](#windows-server-2003)
-   [**ADAM**](#adam)
-   [**Windows Server 2003 R2**](#windows-server-2003-r2)
-   [**Windows Server 2008**](#windows-server-2008)
-   [**Windows Server 2008 R2**](#windows-server-2008-r2)
-   [**Windows Server 2012**](#windows-server-2012)

## <a name="windows-2000-server"></a>Windows 2000 Server



| Ввод | Значение |
|------------------------|-----------------------------------|
| Идентификатор ссылки                | \-                                |
| MAPI-Id                | \-                                |
| System-Only            | Неверно                             |
| Является однозначным       | Верно                              |
| Индексируется             | Неверно                             |
| В глобальном каталоге      | Неверно                             |
| NT-Security-дескриптор | О:БАГ: BAD: S:                      |
| Range-Lower            | \-                                |
| Range-Upper            | \-                                |
| Search-Flags           | 0x00000000                        |
| System-Flags           | 0x00000010                        |
| Классы, используемые в        | [**Пользователь**](c-user.md)<br/> |



## <a name="windows-server-2003"></a>Windows Server 2003



| Ввод | Значение |
|------------------------|-----------------------------------|
| Идентификатор ссылки                | \-                                |
| MAPI-Id                | \-                                |
| System-Only            | Неверно                             |
| Является однозначным       | Верно                              |
| Индексируется             | Неверно                             |
| В глобальном каталоге      | Неверно                             |
| NT-Security-дескриптор | О:БАГ: BAD: S:                      |
| Range-Lower            | \-                                |
| Range-Upper            | \-                                |
| Search-Flags           | 0x00000000                        |
| System-Flags           | 0x00000010                        |
| Классы, используемые в        | [**Пользователь**](c-user.md)<br/> |



## <a name="adam"></a>ADAM



| Ввод | Значение |
|------------------------|-------------------------------------------------------------------|
| Идентификатор ссылки                | \-                                                                |
| MAPI-Id                | \-                                                                |
| System-Only            | Неверно                                                             |
| Является однозначным       | Верно                                                              |
| Индексируется             | Неверно                                                             |
| В глобальном каталоге      | Неверно                                                             |
| NT-Security-дескриптор | О:БАГ: BAD: S:                                                      |
| Range-Lower            | \-                                                                |
| Range-Upper            | \-                                                                |
| Search-Flags           | 0x00000000                                                        |
| System-Flags           | 0x00000010                                                        |
| Классы, используемые в        | [**Объект MS-DS-BIND-Object**](c-msds-bindableobject.md)<br/> |



## <a name="windows-server-2003-r2"></a>Windows Server 2003 R2



| Ввод | Значение |
|------------------------|-----------------------------------|
| Идентификатор ссылки                | \-                                |
| MAPI-Id                | \-                                |
| System-Only            | Неверно                             |
| Является однозначным       | Верно                              |
| Индексируется             | Неверно                             |
| В глобальном каталоге      | Неверно                             |
| NT-Security-дескриптор | О:БАГ: BAD: S:                      |
| Range-Lower            | \-                                |
| Range-Upper            | \-                                |
| Search-Flags           | 0x00000000                        |
| System-Flags           | 0x00000010                        |
| Классы, используемые в        | [**Пользователь**](c-user.md)<br/> |



## <a name="windows-server-2008"></a>Windows Server 2008



| Ввод | Значение |
|------------------------|-----------------------------------|
| Идентификатор ссылки                | \-                                |
| MAPI-Id                | \-                                |
| System-Only            | Неверно                             |
| Является однозначным       | Верно                              |
| Индексируется             | Неверно                             |
| В глобальном каталоге      | Неверно                             |
| NT-Security-дескриптор | О:БАГ: BAD: S:                      |
| Range-Lower            | \-                                |
| Range-Upper            | \-                                |
| Search-Flags           | 0x00000000                        |
| System-Flags           | 0x00000010                        |
| Классы, используемые в        | [**Пользователь**](c-user.md)<br/> |



## <a name="windows-server-2008-r2"></a>Windows Server 2008 R2



| Ввод | Значение |
|------------------------|-----------------------------------|
| Идентификатор ссылки                | \-                                |
| MAPI-Id                | \-                                |
| System-Only            | Неверно                             |
| Является однозначным       | Верно                              |
| Индексируется             | Неверно                             |
| В глобальном каталоге      | Неверно                             |
| NT-Security-дескриптор | О:БАГ: BAD: S:                      |
| Range-Lower            | \-                                |
| Range-Upper            | \-                                |
| Search-Flags           | 0x00000000                        |
| System-Flags           | 0x00000010                        |
| Классы, используемые в        | [**Пользователь**](c-user.md)<br/> |



## <a name="windows-server-2012"></a>Windows Server 2012



| Ввод | Значение |
|------------------------|-----------------------------------|
| Идентификатор ссылки                | \-                                |
| MAPI-Id                | \-                                |
| System-Only            | Неверно                             |
| Является однозначным       | Верно                              |
| Индексируется             | Неверно                             |
| В глобальном каталоге      | Неверно                             |
| NT-Security-дескриптор | О:БАГ: BAD: S:                      |
| Range-Lower            | \-                                |
| Range-Upper            | \-                                |
| Search-Flags           | 0x00000000                        |
| System-Flags           | 0x00000010                        |
| Классы, используемые в        | [**Пользователь**](c-user.md)<br/> |



## <a name="remarks"></a>Remarks

Большая часть этого большого целого числа соответствует элементу **двхигхдатетиме** структуры [**fileTime**](/windows/desktop/api/minwinbase/ns-minwinbase-filetime) , а нижняя часть соответствует элементу **двловдатетиме** структуры **fileTime** .

## <a name="see-also"></a>См. также

<dl> <dt>

[**Управление учетными записями пользователей**](a-useraccountcontrol.md)
</dt> </dl>

 

