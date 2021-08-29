---
title: С прекращением использования-REPL-DSA-сигнатуры
description: Отслеживает удостоверения предыдущей репликации DS для данного контроллера домена.
ms.assetid: 82e8b222-5635-41ad-b2ab-386c9e6aa280
ms.tgt_platform: multiple
keywords:
- С прекращением использования-REPL-DSA-схема AD атрибутов сигнатур
- Схема AD атрибута Ретиредреплдсасигнатурес
topic_type:
- apiref
api_name:
- Retired-Repl-DSA-Signatures
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d0521644304cef0af7d0b1ba01b582e5b5ae64b1921736925008e7394e4b1a46
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119646904"
---
# <a name="retired-repl-dsa-signatures-attribute"></a>С прекращением использования-REPL-DSA-сигнатуры

Отслеживает удостоверения предыдущей репликации DS для данного контроллера домена.



| Ввод | Значение |
|-------------------|-------------------------------------------------------------------------------------|
| CN                | Отменено-REPL-DSA-Signatures                                                         |
| LDAP-отображаемое имя | ретиредреплдсасигнатурес                                                            |
| Размер              | Длина пропорциональна количеству восстановлений контроллера домена из резервной копии. |
| Привилегия обновления  | Это значение задается системой.                                                    |
| Частота обновления  | \-                                                                                  |
| Attribute-Id      | 1.2.840.113556.1.4.673                                                              |
| System-ID — GUID    | 7bfdcb7f-4807-11d1-a9c3-0000f80367c1                                                |
| Синтаксис            | [**Object(ссылка_на_реплику)**](s-object-replica-link.md)                               |



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
|------------------------|------------------------------------------|
| Идентификатор ссылки                | \-                                       |
| MAPI-Id                | \-                                       |
| System-Only            | Верно                                     |
| Является однозначным       | Верно                                     |
| Индексируется             | Нет                                    |
| В глобальном каталоге      | Нет                                    |
| NT-Security-дескриптор | О:БАГ: BAD: S:                             |
| Range-Lower            | \-                                       |
| Range-Upper            | \-                                       |
| Search-Flags           | 0x00000000                               |
| System-Flags           | 0x00000010                               |
| Классы, используемые в        | [**NTDS-DSA**](c-ntdsdsa.md)<br/> |



## <a name="windows-server-2003"></a>Windows Server 2003



| Ввод | Значение |
|------------------------|------------------------------------------|
| Идентификатор ссылки                | \-                                       |
| MAPI-Id                | \-                                       |
| System-Only            | Верно                                     |
| Является однозначным       | Верно                                     |
| Индексируется             | Нет                                    |
| В глобальном каталоге      | Нет                                    |
| NT-Security-дескриптор | О:БАГ: BAD: S:                             |
| Range-Lower            | \-                                       |
| Range-Upper            | \-                                       |
| Search-Flags           | 0x00000000                               |
| System-Flags           | 0x00000010                               |
| Классы, используемые в        | [**NTDS-DSA**](c-ntdsdsa.md)<br/> |



## <a name="adam"></a>ADAM



| Ввод | Значение |
|------------------------|------------------------------------------|
| Идентификатор ссылки                | \-                                       |
| MAPI-Id                | \-                                       |
| System-Only            | Верно                                     |
| Является однозначным       | Верно                                     |
| Индексируется             | Нет                                    |
| В глобальном каталоге      | Нет                                    |
| NT-Security-дескриптор | О:БАГ: BAD: S:                             |
| Range-Lower            | \-                                       |
| Range-Upper            | \-                                       |
| Search-Flags           | 0x00000000                               |
| System-Flags           | 0x00000010                               |
| Классы, используемые в        | [**NTDS-DSA**](c-ntdsdsa.md)<br/> |



## <a name="windows-server-2003-r2"></a>Windows Server 2003 R2



| Ввод | Значение |
|------------------------|------------------------------------------|
| Идентификатор ссылки                | \-                                       |
| MAPI-Id                | \-                                       |
| System-Only            | Верно                                     |
| Является однозначным       | Верно                                     |
| Индексируется             | Нет                                    |
| В глобальном каталоге      | Нет                                    |
| NT-Security-дескриптор | О:БАГ: BAD: S:                             |
| Range-Lower            | \-                                       |
| Range-Upper            | \-                                       |
| Search-Flags           | 0x00000000                               |
| System-Flags           | 0x00000010                               |
| Классы, используемые в        | [**NTDS-DSA**](c-ntdsdsa.md)<br/> |



## <a name="windows-server-2008"></a>Windows Server 2008



| Ввод | Значение |
|------------------------|------------------------------------------|
| Идентификатор ссылки                | \-                                       |
| MAPI-Id                | \-                                       |
| System-Only            | Верно                                     |
| Является однозначным       | Верно                                     |
| Индексируется             | Нет                                    |
| В глобальном каталоге      | Нет                                    |
| NT-Security-дескриптор | О:БАГ: BAD: S:                             |
| Range-Lower            | \-                                       |
| Range-Upper            | \-                                       |
| Search-Flags           | 0x00000000                               |
| System-Flags           | 0x00000010                               |
| Классы, используемые в        | [**NTDS-DSA**](c-ntdsdsa.md)<br/> |



## <a name="windows-server-2008-r2"></a>Windows Server 2008 R2



| Ввод | Значение |
|------------------------|------------------------------------------|
| Идентификатор ссылки                | \-                                       |
| MAPI-Id                | \-                                       |
| System-Only            | Верно                                     |
| Является однозначным       | Верно                                     |
| Индексируется             | Нет                                    |
| В глобальном каталоге      | Нет                                    |
| NT-Security-дескриптор | О:БАГ: BAD: S:                             |
| Range-Lower            | \-                                       |
| Range-Upper            | \-                                       |
| Search-Flags           | 0x00000000                               |
| System-Flags           | 0x00000010                               |
| Классы, используемые в        | [**NTDS-DSA**](c-ntdsdsa.md)<br/> |



## <a name="windows-server-2012"></a>Windows Server 2012



| Ввод | Значение |
|------------------------|------------------------------------------|
| Идентификатор ссылки                | \-                                       |
| MAPI-Id                | \-                                       |
| System-Only            | Верно                                     |
| Является однозначным       | Верно                                     |
| Индексируется             | Нет                                    |
| В глобальном каталоге      | Нет                                    |
| NT-Security-дескриптор | О:БАГ: BAD: S:                             |
| Range-Lower            | \-                                       |
| Range-Upper            | \-                                       |
| Search-Flags           | 0x00000000                               |
| System-Flags           | 0x00000010                               |
| Классы, используемые в        | [**NTDS-DSA**](c-ntdsdsa.md)<br/> |



 

 





