---
description: Записывает значение слова в указанную базу данных.
ms.assetid: 8f921e14-4a82-4d8e-83fa-beb78118ecb8
title: Функция Сдбвритевордтаг
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SdbWriteWORDTag
api_type:
- DllExport
api_location:
- Apphelp.dll
ms.openlocfilehash: a511b4a0ef738a6b5e11c797780e30c68be5eb4e9dad62cecf66e1998c2e1383
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120044754"
---
# <a name="sdbwritewordtag-function"></a>Функция Сдбвритевордтаг

Записывает значение **слова** в указанную базу данных.

## <a name="syntax"></a>Синтаксис


```C++
BOOL WINAPI SdbWriteWORDTag(
  _In_ PDB  pdb,
  _In_ TAG  tTag,
  _In_ WORD wData
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

ТЕГ для записи. Этот тег должен иметь тип **тега \_ \_ Word**.

</dd> <dt>

*вдата* \[ окне\]
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

[**сдбвритеквордтаг**](sdbwriteqwordtag.md)
</dt> <dt>

[**сдбвритестрингтаг**](sdbwritestringtag.md)
</dt> </dl>

 

 




