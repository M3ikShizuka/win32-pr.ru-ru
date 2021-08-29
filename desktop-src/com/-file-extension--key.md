---
title: Ключ file_extension
description: Связывает расширение имени файла с ProgID.
ms.assetid: 018998a8-c0da-43ea-bae2-3b184897eb9b
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3d7624b63d257e0d0edf168956c862c911ba728da955e8eea3ca54f6ce452878
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120071234"
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

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**FileType**](filetype-key.md)
</dt> <dt>

[**жетклассфиле**](/windows/desktop/api/Objbase/nf-objbase-getclassfile)
</dt> </dl>

 

 




