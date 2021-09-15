---
description: Абстрактный базовый класс, из которого производятся все классы данных поставщика (MCA), например Мсмкаинфо \_ равмкадата. этот класс доступен только в 64-разрядных Windows системах.
ms.assetid: 22ec8343-fc4f-4b14-9354-26b5d6a6fe09
title: Класс Мсмкаинфо
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- MSMCAInfo
api_type:
- DllExport
api_location:
- Wmiprov.dll
ms.openlocfilehash: 31fc35b1d680d900af929ea8a828bcb23d222f66
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127568103"
---
# <a name="msmcainfo-class"></a>Класс Мсмкаинфо

Класс **мсмкаинфо** является абстрактным базовым классом, из которого производятся все классы данных поставщика (например, [**мсмкаинфо \_ равмкадата**](msmcainfo-rawmcadata.md)). Поставщик MCA также имеет классы событий, производные от [**WMIEvent**](wmievent.md). этот класс доступен только в 64-разрядных Windows системах.

Следующий синтаксис упрощен из кода MOF-файл (MOF) и включает все его унаследованные свойства. Свойства и методы имеют алфавитный порядок, а не порядок MOF.

## <a name="syntax"></a>Синтаксис

``` syntax
class MSMCAInfo
{
};
```

## <a name="members"></a>Участники

Класс **мсмкаинфо** не определяет никаких членов.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP<br/>                                                                  |
| Минимальная версия сервера<br/> | Windows Server 2003<br/>                                                         |
| Пространство имен<br/>                | Корневой \\ инструментарий WMI<br/>                                                                   |
| MOF<br/>                      | <dl> <dt>Вмикоре. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Wmiprov.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Классы МСМКА](msmca-classes.md)
</dt> <dt>

[**\_Заголовок мсмкаевент**](msmcaevent-header.md)
</dt> <dt>

[**WMIEvent**](wmievent.md)
</dt> </dl>

 

 




