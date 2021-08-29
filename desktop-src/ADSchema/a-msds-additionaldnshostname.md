---
title: Атрибут ms-DS-дополнительно-DNS-Host-Name
description: Атрибут используется для хранения дополнительного имени узла DNS для объекта-компьютера. Этот атрибут используется во время переименования контроллера домена.
ms.assetid: ea06f756-d9b6-409d-a008-0e3a1874ad94
ms.tgt_platform: multiple
keywords:
- Схема AD для атрибута ms-DS-дополнительно-DNS-Host-Name
- Схема AD атрибута msDS-Аддитионалдншостнаме
topic_type:
- apiref
api_name:
- ms-DS-Additional-Dns-Host-Name
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 957829d688b1b89af59695a7929ed89d004fe2de9b7bf04c4478ad008f88a57b
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119804234"
---
# <a name="ms-ds-additional-dns-host-name-attribute"></a>Атрибут ms-DS-дополнительно-DNS-Host-Name

Атрибут используется для хранения дополнительного имени узла DNS для объекта-компьютера. Этот атрибут используется во время переименования компьютера или управления именами с помощью "Netdom ComputerName".



| Ввод | Значение |
|-------------------|-----------------------------------------------------------------------------|
| CN                | MS-DS-дополнительно-DNS-Host-Name                                              |
| LDAP-отображаемое имя | msDS-Аддитионалдншостнаме                                                  |
| Размер              | Каждое значение может содержать 2048 символов. Количество значений — это ограничение базы данных, равное 1200. |
| Привилегия обновления  | Это значение задается системой.                                            |
| Частота обновления  | При переименовании компьютера.                                                 |
| Attribute-Id      | 1.2.840.113556.1.4.1717                                                     |
| System-ID — GUID    | 80863791-dbe9-4eb8-837e-7f0ab55d9ac7                                        |
| Синтаксис            | [**String(Юникод)**](s-string-unicode.md)                                 |



## <a name="implementations"></a>Варианты реализации решения

-   [**Windows Server 2003**](#windows-server-2003)
-   [**Windows Server 2003 R2**](#windows-server-2003-r2)
-   [**Windows Server 2008**](#windows-server-2008)
-   [**Windows Server 2008 R2**](#windows-server-2008-r2)
-   [**Windows Server 2012**](#windows-server-2012)

## <a name="windows-server-2003"></a>Windows Server 2003



| Ввод | Значение |
|------------------------|-------------------------------------------|
| Идентификатор ссылки                | \-                                        |
| MAPI-Id                | \-                                        |
| System-Only            | Верно                                      |
| Является однозначным       | Нет                                     |
| Индексируется             | Нет                                     |
| В глобальном каталоге      | Нет                                     |
| NT-Security-дескриптор | О:БАГ: BAD: S:                              |
| Range-Lower            | 0                                         |
| Range-Upper            | 2048                                      |
| Search-Flags           | 0x00000000                                |
| System-Flags           | 0x00000010                                |
| Классы, используемые в        | [**Компьютер**](c-computer.md)<br/> |



## <a name="windows-server-2003-r2"></a>Windows Server 2003 R2



| Ввод | Значение |
|------------------------|-------------------------------------------|
| Идентификатор ссылки                | \-                                        |
| MAPI-Id                | \-                                        |
| System-Only            | Верно                                      |
| Является однозначным       | Нет                                     |
| Индексируется             | Нет                                     |
| В глобальном каталоге      | Нет                                     |
| NT-Security-дескриптор | О:БАГ: BAD: S:                              |
| Range-Lower            | 0                                         |
| Range-Upper            | 2048                                      |
| Search-Flags           | 0x00000000                                |
| System-Flags           | 0x00000010                                |
| Классы, используемые в        | [**Компьютер**](c-computer.md)<br/> |



## <a name="windows-server-2008"></a>Windows Server 2008



| Ввод | Значение |
|------------------------|-------------------------------------------|
| Идентификатор ссылки                | \-                                        |
| MAPI-Id                | \-                                        |
| System-Only            | Верно                                      |
| Является однозначным       | Нет                                     |
| Индексируется             | Нет                                     |
| В глобальном каталоге      | Нет                                     |
| NT-Security-дескриптор | О:БАГ: BAD: S:                              |
| Range-Lower            | 0                                         |
| Range-Upper            | 2048                                      |
| Search-Flags           | 0x00000000                                |
| System-Flags           | 0x00000010                                |
| Классы, используемые в        | [**Компьютер**](c-computer.md)<br/> |



## <a name="windows-server-2008-r2"></a>Windows Server 2008 R2



| Ввод | Значение |
|------------------------|-------------------------------------------|
| Идентификатор ссылки                | \-                                        |
| MAPI-Id                | \-                                        |
| System-Only            | Верно                                      |
| Является однозначным       | Нет                                     |
| Индексируется             | Нет                                     |
| В глобальном каталоге      | Нет                                     |
| NT-Security-дескриптор | О:БАГ: BAD: S:                              |
| Range-Lower            | 0                                         |
| Range-Upper            | 2048                                      |
| Search-Flags           | 0x00000000                                |
| System-Flags           | 0x00000010                                |
| Классы, используемые в        | [**Компьютер**](c-computer.md)<br/> |



## <a name="windows-server-2012"></a>Windows Server 2012



| Ввод | Значение |
|------------------------|-------------------------------------------|
| Идентификатор ссылки                | \-                                        |
| MAPI-Id                | \-                                        |
| System-Only            | Верно                                      |
| Является однозначным       | Нет                                     |
| Индексируется             | Нет                                     |
| В глобальном каталоге      | Нет                                     |
| NT-Security-дескриптор | О:БАГ: BAD: S:                              |
| Range-Lower            | 0                                         |
| Range-Upper            | 2048                                      |
| Search-Flags           | 0x00000000                                |
| System-Flags           | 0x00000010                                |
| Классы, используемые в        | [**Компьютер**](c-computer.md)<br/> |



 

 





