---
title: Ключ file_extension
description: Связывает расширение имени файла с ProgID.
ms.assetid: 018998a8-c0da-43ea-bae2-3b184897eb9b
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e602266f3c851975c2f8e008ced5dfc8e2d40b64
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369605"
---
# <a name="file_extension-key"></a><\_> ключ расширения файла

Связывает расширение имени файла с ProgID.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes
   .ext = ProgID
```

## <a name="remarks"></a>Remarks

сведения, содержащиеся в ключе расширения имени файла, используются как в обозревателе Windows, так и в моникерах файлов. [**Жетклассфиле**](/windows/desktop/api/Objbase/nf-objbase-getclassfile) использует ключ расширения имени файла для предоставления связанного идентификатора CLSID.

Ключ **\_ \_ \\ \\ классов программного обеспечения файла hKey на локальном компьютере** соответствует **\_ \_ корневому ключу classes** , который был сохранен для совместимости с предыдущими версиями com.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[**FileType**](filetype-key.md)
</dt> <dt>

[**жетклассфиле**](/windows/desktop/api/Objbase/nf-objbase-getclassfile)
</dt> </dl>

 

 




