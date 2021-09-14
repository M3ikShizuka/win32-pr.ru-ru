---
title: инпроксервер
description: Указывает путь к DLL внутрипроцессного сервера.
ms.assetid: f14cc8f7-e93e-4db8-8b0d-ea77a6301f33
keywords:
- COM раздела реестра Инпроксервер
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5682693d711f734bbc60def8a711f11e2bad0ef9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053159"
---
# <a name="inprocserver"></a>инпроксервер

Указывает путь к DLL внутрипроцессного сервера.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID
   {CLSID}
      InprocServer
         (Default) = path
```

## <a name="remarks"></a>Комментарии

Запись **инпроксервер** сравнительно редко используется для вставляемых классов.

Внутрипроцессный сервер в настоящее время зарегистрирован с помощью записи реестра **инпроксервер** . 32-разрядные и 64-битные внутрипроцессный серверы должны использовать запись [**InprocServer32**](inprocserver32.md) . Если контейнер выполняет поиск в реестре внутрипроцессного сервера, 16-разрядная версия имеет приоритет с 16-разрядным контейнером, а 32-разрядная версия имеет приоритет с 32-битным контейнером.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**InprocServer32**](inprocserver32.md)
</dt> </dl>

 

 




