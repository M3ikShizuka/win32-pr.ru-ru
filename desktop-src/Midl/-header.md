---
title: /Header, параметр
description: Параметр/header указывает имя файла заголовка.
ms.assetid: d36cb6c9-df57-4ef4-aff3-9968ac8ac001
keywords:
- MIDL/Header Switch
topic_type:
- apiref
api_name:
- /header
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 816310f0b584f3c30d351e0d036e1f18c2f23962
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127144181"
---
# <a name="header-switch"></a>/Header, параметр

Параметр **/Header** указывает имя файла заголовка.

``` syntax
midl /header filename
```

## <a name="switch-options"></a>Параметры коммутатора

<dl> <dt>

*filename* 
</dt> <dd>

Задает имя файла заголовка, переопределяющего имя файла заголовка по умолчанию. Имена файлов можно явно заключить в кавычки с помощью двойных кавычек ("), чтобы оболочка не могла интерпретировать специальные символы.

</dd> </dl>

## <a name="remarks"></a>Remarks

Указанное имя файла заменяет имя файла по умолчанию. Имя файла по умолчанию получается путем замены расширения IDL (обычно IDL) именем файла Extension. h. Для интерфейсов OLE параметр **/Header** переопределяет имя файла заголовка интерфейса по умолчанию.

При импорте файлов указанное имя файла применяется только к одному файлу заголовка — файлу заголовка, соответствующему IDL-файлу, указанному в командной строке.

Если *имя_файла* не включает явный путь, файл записывается в текущий каталог или в каталог, указанный параметром [**/out**](-out.md) . Явный путь в *filename* переопределяет спецификацию переключателя **/out** .

## <a name="examples"></a>Примеры

**MIDL/Header "Bar. h" имя_файла. idl**

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Общий синтаксис командной строки MIDL](general-midl-command-line-syntax.md)
</dt> <dt>

[**/h**](-h.md)
</dt> <dt>

[**/cstub**](-cstub.md)
</dt> <dt>

[**/out**](-out.md)
</dt> <dt>

[**/sstub**](-sstub.md)
</dt> <dt>

[**/Proxy**](-proxy.md)
</dt> </dl>

 

 




