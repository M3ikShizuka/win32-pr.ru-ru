---
title: InprocHandler32
description: InprocHandler32 указывает, использует ли приложение настраиваемый обработчик в HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID разделе реестра.
ms.assetid: da611bb6-1f69-449a-9821-e2fbbe413a97
keywords:
- COM раздела реестра InprocHandler32
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: be73a8b2577a554b0bb8b5ba5a851e630edbf90a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053160"
---
# <a name="inprochandler32"></a>InprocHandler32

Указывает, использует ли приложение пользовательский обработчик.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID
   {CLSID}
      InprocHandler32 = handler.dll
```

## <a name="remarks"></a>Комментарии

Это значение **reg \_ SZ** , указывающее настраиваемый обработчик, используемый приложением. Если пользовательский обработчик не используется, для записи следует задать значение Ole32.dll.

Если контейнер выполняет поиск пользовательского обработчика в реестре, 16-разрядная версия имеет приоритет с 16-разрядным контейнером, а 32-разрядная версия имеет приоритет с 32-битным контейнером.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**инпрочандлер**](inprochandler.md)
</dt> </dl>

 

 




