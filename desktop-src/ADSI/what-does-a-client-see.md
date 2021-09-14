---
title: Что видят клиенты
description: В этом разделе перечислены способы, с помощью которых клиент просматривает данные ADSI.
ms.assetid: 238eeea9-1303-4d37-bf09-ad03f1790c1b
ms.tgt_platform: multiple
keywords:
- расширения ADSI, что видят клиенты
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 398c9fd2d603c1eebb18280c435bec7cb7cd8e14
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126970377"
---
# <a name="what-does-a-client-see"></a>Что видят клиенты?

-   Клиент видит ADSI и все его объекты расширения как один объект.
-   Клиент ADSI видит один интерфейс [**IDispatch**](/windows/win32/api/oaidl/nn-oaidl-idispatch) , который обрабатывает все сдвоенные и отправляемые интерфейсы в объекте, независимо от того, реализуется ли сдвоенный или исправный интерфейс агрегатором в поставщике или расширением. Ознакомьтесь с [разрешениями конфликтов имен функций и свойств в службе автоматизации в расширениях](resolution-of-functionproperty-name-conflicts-in-automation-in-extensions.md).
-   ADSI не предоставляет никаких сведений о типе с помощью методов [**IDispatch:: GetTypeInfo**](/windows/win32/api/oaidl/nf-oaidl-idispatch-gettypeinfo) или [**IDispatch:: жеттипеинфокаунт**](/windows/win32/api/oaidl/nf-oaidl-idispatch-gettypeinfocount) . ADSI предоставляет сведения о типах с помощью библиотеки типов.

 

 