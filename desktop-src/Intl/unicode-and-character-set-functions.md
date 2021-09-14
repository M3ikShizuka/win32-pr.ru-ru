---
description: Для наборов символов используются следующие функции.
ms.assetid: 1799f5da-1391-4b6e-ac13-718017a77557
title: Функции Юникода и кодировка символов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6996139d8a9bb426c21a460ac2bcb1358e6c8e7c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127255004"
---
# <a name="unicode-and-character-set-functions"></a>Функции Юникода и кодировка символов

Для наборов символов используются следующие функции.



| Функция                                                       | Описание                                                                                                           |
|----------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| [**жеттекстчарсет**](/windows/desktop/api/Wingdi/nf-wingdi-gettextcharset)                       | Извлекает идентификатор кодировки для шрифта, выбранного в данный момент в указанном контексте устройства.         |
| [**жеттекстчарсетинфо**](/windows/desktop/api/Wingdi/nf-wingdi-gettextcharsetinfo)               | Извлекает сведения о кодировке шрифта, выбранного в данный момент в указанном контексте устройства. |
| [**исдбкслеадбите**](/windows/desktop/api/Winnls/nf-winnls-isdbcsleadbyte)                       | определяет, является ли указанный символ старшим байтом для системной кодовой страницы по умолчанию Windows ANSI (CP \_ ACP).           |
| [**исдбкслеадбитикс**](/windows/desktop/api/Winnls/nf-winnls-isdbcsleadbyteex)                   | Определяет, является ли указанный символ потенциально старшим байтом.                                                       |
| [**истекстуникоде**](/windows/desktop/api/Winbase/nf-winbase-istextunicode)                         | Определяет, может ли буфер содержать форму текста в Юникоде.                                                   |
| [**MultiByteToWideChar**](/windows/desktop/api/Stringapiset/nf-stringapiset-multibytetowidechar)             | Карты строку символов в строку UTF-16 (расширенная кодировка).                                                          |
| [**транслатечарсетинфо**](/windows/desktop/api/Wingdi/nf-wingdi-translatecharsetinfo)           | Преобразует сведения о кодировке и задает соответствующие значения для всех элементов целевой структуры.           |
| [**WideCharToMultiByte**](/windows/desktop/api/Stringapiset/nf-stringapiset-widechartomultibyte)             | Карты строку UTF-16 (расширенных символов) в новую строку символов.                                                      |
| [**битестауникоде**](/previous-versions/dd317724(v=vs.85))                       | Не используйте.                                                                                                           |
| [**нлсдллкодепажетранслатион**](/windows/desktop/api/Gb18030/nf-gb18030-nlsdllcodepagetranslation) | Не используйте.                                                                                                           |
| [**уникодетобитес**](/previous-versions/windows/desktop/legacy/dd374082(v=vs.85))                       | Не используется.                                                                                                           |



 

 

 
