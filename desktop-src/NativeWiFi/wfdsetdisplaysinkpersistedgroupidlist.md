---
description: Задает список идентификаторов сохраненной группы для всех профилей, сохраняемых приложением.
ms.assetid: EF83F295-CD53-45A4-B209-560B4069CA7C
title: Функция Вфддисплайсинксетперсистедграупидлист (Вфдсинк. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- WFDSetDisplaySinkPersistedGroupIDList
api_type:
- DllExport
api_location:
- wifidisplay.dll
ms.openlocfilehash: ce31b6e4bf6336baede3767d3457f44d92dde0e39f6418bcc3c2529b644fe24c
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119800394"
---
# <a name="wfddisplaysinksetpersistedgroupidlist-function"></a>Функция Вфддисплайсинксетперсистедграупидлист

Задает список идентификаторов сохраненной группы для всех профилей, сохраняемых приложением. Приложение должно вызывать этот метод при каждом добавлении или удалении профиля из своего хранилища.

## <a name="syntax"></a>Синтаксис


```C++
DWORD WINAPI WFDSetDisplaySinkPersistedGroupIDList(
  _In_ UINT32             cGroupIDList,
  _In_ DOT11_WFD_GROUP_ID *pGroupIDList
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*кграупидлист* \[ окне\]
</dt> <dd>

Число идентификаторов групп, на которые указывает *пграупидлист*.

</dd> <dt>

*пграупидлист* \[ окне\]
</dt> <dd>

Указатель на массив идентификаторов групп *кграупидлист* .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если функция завершается успешно, возвращается значение ошибки \_ Success.

## <a name="remarks"></a>Remarks

Этот метод всегда должен вызываться со всем списком, а не подмножеством. Этот метод можно вызывать с 0 профилями, если хранилище профиля пусто.

Вызов повторного вызова для идентификатора группы, не входящего в предоставленный список, завершится ошибкой "Failed; неизвестная группа P2P "(состояние 8).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                               |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                                    |
| Окончание поддержки клиента<br/>    | Windows 10,<br/>                                                                      |
| Поддержка конца сервера<br/>    | Windows Server 2016<br/>                                                             |
| Заголовок<br/>                   | <dl> <dt>Вфдсинк. h</dt> </dl>       |
| Библиотека<br/>                  | <dl> <dt>Вифидисплай. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Wifidisplay.dll</dt> </dl> |



 

 




