---
description: Записывает значение QWORD в указанную базу данных.
ms.assetid: 8ce566ea-a941-45fa-b031-26c3144ca02c
title: Функция Сдбвритеквордтаг
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SdbWriteQWORDTag
api_type:
- DllExport
api_location:
- Apphelp.dll
ms.openlocfilehash: adff37c575604f9d717c3e2253c9cad545a14c32e22c7718c9063384c78a37b4
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120044784"
---
# <a name="sdbwriteqwordtag-function"></a>Функция Сдбвритеквордтаг

Записывает значение **QWORD** в указанную базу данных.

## <a name="syntax"></a>Синтаксис


```C++
BOOL WINAPI SdbWriteQWORDTag(
  _In_ PDB       pdb,
  _In_ TAG       tTag,
  _In_ ULONGLONG qwData
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pdb* \[ -файл окне\]
</dt> <dd>

Маркер базы данных оболочек совместимости.

</dd> <dt>

*ттаг* \[ окне\]
</dt> <dd>

ТЕГ для записи. Этот тег должен иметь тип **тега \_ \_ QWORD**.

</dd> <dt>

*квдата* \[ окне\]
</dt> <dd>

Значение.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Функция возвращает **true** при успешном выполнении или **false** в случае сбоя.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                   |
| DLL<br/>                      | <dl> <dt>Apphelp.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**сдбвритебинаритаг**](sdbwritebinarytag.md)
</dt> <dt>

[**сдбвритедвордтаг**](sdbwritedwordtag.md)
</dt> <dt>

[**сдбвритестрингтаг**](sdbwritestringtag.md)
</dt> <dt>

[**сдбвритевордтаг**](sdbwritewordtag.md)
</dt> </dl>

 

 




