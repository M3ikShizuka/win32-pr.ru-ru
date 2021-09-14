---
title: локалсервер
description: Указывает полный путь к 16-разрядному приложению локального сервера.
ms.assetid: 6eadadd5-f4d3-4e0d-9491-2ea366861aa7
keywords:
- COM раздела реестра Локалсервер
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7413f9d7c4d17e9498e80d19b70192fbb21911b6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127249283"
---
# <a name="localserver"></a>локалсервер

Указывает полный путь к 16-разрядному приложению локального сервера.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID
   {CLSID}
      LocalServer = path
```

## <a name="remarks"></a>Комментарии

Это значение **reg \_ SZ** , которое указывает полный путь и может содержать любые аргументы командной строки.

COM добавляет к строке флаг "-Встраивание", поэтому приложение, использующее флаги, должно проанализировать всю строку и проверить флаг-встраивание.

Чтобы запустить сервер COM Object Server в отдельной области памяти, измените значение **локалсервер** следующим образом:

**cmd/c запуск/сепарате** *путь * * * .exe**

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**LocalServer32**](localserver32.md)
</dt> </dl>

 

 




