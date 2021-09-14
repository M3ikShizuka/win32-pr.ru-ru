---
description: Структура ПРОВИДОР \_ info \_ 1 определяет поставщика печати.
ms.assetid: 0eff115a-b3d2-4c8f-b820-46e7f62dd295
title: Структура PROVIDOR_INFO_1 (Винспул. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PROVIDOR_INFO_1
- _PROVIDOR_INFO_1A
- _PROVIDOR_INFO_1W
api_type:
- HeaderDef
api_location:
- Winspool.h
ms.openlocfilehash: 2eabc00009b76247af71b06ea877ca0bf738c1d5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127248395"
---
# <a name="providor_info_1-structure"></a>\_Структура провидор info \_ 1

Структура **провидор \_ info \_ 1** определяет поставщика печати.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _PROVIDOR_INFO_1 {
  LPTSTR pName;
  LPTSTR pEnvironment;
  LPTSTR pDLLName;
} PROVIDOR_INFO_1, *PPROVIDOR_INFO_1;
```



## <a name="members"></a>Участники

<dl> <dt>

**pName**
</dt> <dd>

Указатель на строку, завершающуюся нулем, которая является именем поставщика печати.

</dd> <dt>

**пенвиронмент**
</dt> <dd>

Указатель на строку среды, заканчивающуюся нулем, указывающую среду, которую библиотека динамической компоновки (DLL) поставщика поддерживает для запуска.

</dd> <dt>

**пдллнаме**
</dt> <dd>

Указатель на строку, завершающуюся нулем, которая является именем поставщика, .dll.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>винспул. h (включает Windows. h)</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **\_ \_ Сведения о провидор \_ 1W** (Юникод) и **\_ провидор \_ info \_ 1A** (ANSI)<br/>                         |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Вывод на печать](printdocs-printing.md)
</dt> <dt>

[Структуры API диспетчера очереди печати](printing-and-print-spooler-structures.md)
</dt> <dt>

[**аддпринтпровидор**](addprintprovidor.md)
</dt> </dl>

 

 




