---
title: /LCID, параметр
description: Параметр компилятора/LCID MIDL позволяет использовать международные символы во входных файлах, именах файлов и путях к каталогам.
ms.assetid: 2ab4ba67-4414-4889-8ed7-83f4888caf8b
keywords:
- MIDL/LCID Switch
topic_type:
- apiref
api_name:
- /lcid
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 370548bb9899ce84173f2321a129aaeda1c6fe81
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127144165"
---
# <a name="lcid-switch"></a>/LCID, параметр

Параметр компилятора **/LCID** MIDL позволяет использовать международные символы во входных файлах, именах файлов и путях к каталогам.

``` syntax
midl /lcid localeID
```

## <a name="switch-options"></a>Параметры коммутатора

<dl> <dt>

*localeID* 
</dt> <dd>

указывает 32-разрядный идентификатор локали, используемый в Windows поддержки национальных языков. Код локали должен быть указан в десятичном формате.

</dd> </dl>

## <a name="remarks"></a>Remarks

Во входных файлах можно использовать локализованные комментарии, строки, хелпстрингс и идентификаторы. В частности, параметр **/LCID** обеспечивает полную поддержку DBCS для представления азиатских языков, таких как японский, китайский и корейский.

> [!Note]  
> Параметр **/LCID** доступен в MIDL версии 3.01.75 и более поздних.

 

## <a name="examples"></a>Примеры

**MIDL/LCID 1041 iface. idl**

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Общий синтаксис командной строки MIDL](general-midl-command-line-syntax.md)
</dt> <dt>

[**намного**](lcid.md)
</dt> </dl>

 

 




