---
title: DataFormats
description: Указывает форматы данных по умолчанию и основные параметры, поддерживаемые приложением.
ms.assetid: 0c9387f9-d7e0-40e7-8d86-96a79a844161
keywords:
- Формат COM раздела реестра
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: bf130461a8db67cfe7fc7c56b0115b27eef6dc6b
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369574"
---
# <a name="dataformats"></a>DataFormats

Указывает форматы данных по умолчанию и основные параметры, поддерживаемые приложением.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID
   {CLSID}
      DataFormats
         DefaultFile = file/format
         GetSet
            n = formats
```

## <a name="remarks"></a>Remarks

Значение *File/Format* указывает основной файл или формат объекта по умолчанию для объектов этого класса.

Значение *formats* указывает список форматов для реализаций по умолчанию [**енумформатетк**](/windows/desktop/api/ObjIdl/nf-objidl-idataobject-enumformatetc), где *n* — целочисленный индекс, начинающийся с нуля. Например, *n*  =  *Format*, *аспект*, *средний*, *флаг*, где *Формат* — формат буфера обмена, *аспект* — один или несколько членов [**дваспект**](/windows/win32/api/wtypes/ne-wtypes-dvaspect), *средний* — один или несколько членов [**тимед**](/windows/win32/api/objidl/ne-objidl-tymed), а *флаг* — один или несколько элементов [**DATADIR**](/windows/win32/api/objidl/ne-objidl-datadir).

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[**IDataObject:: Енумформатетк**](/windows/desktop/api/ObjIdl/nf-objidl-idataobject-enumformatetc)
</dt> <dt>

[**IDataObject:: GetData**](/windows/desktop/api/ObjIdl/nf-objidl-idataobject-getdata)
</dt> <dt>

[**IDataObject:: SetData**](/windows/desktop/api/ObjIdl/nf-objidl-idataobject-setdata)
</dt> </dl>

 

 




