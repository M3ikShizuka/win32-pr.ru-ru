---
title: Структура MCI_OPEN_PARMS (МЦиапи. h)
description: Структура MCI \_ Open \_ пармс содержит сведения для \_ команды MCI Open.
ms.assetid: d22cefeb-3d49-47cf-a946-f73c77ae43fd
keywords:
- структура MCI_OPEN_PARMS Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_OPEN_PARMS
api_location:
- mciapi.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 658f97a9b2677347c9818265c1f05c2115c95fdd
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370023"
---
# <a name="mci_open_parms-structure"></a>\_Структура Open \_ ПАРМС для MCI

Структура **MCI \_ Open \_ пармс** содержит сведения для команды [**MCI \_ Open**](mci-open.md) .

## <a name="syntax"></a>Синтаксис


```C++
typedef struct {
  DWORD_PTR   dwCallback;
  MCIDEVICEID wDeviceID;
  LPCTSTR     lpstrDeviceType;
  LPCTSTR     lpstrElementName;
  LPCTSTR     lpstrAlias;
} MCI_OPEN_PARMS;
```



## <a name="members"></a>Участники

<dl> <dt>

**двкаллбакк**
</dt> <dd>

Слово нижнего порядка задает маркер окна, используемый для \_ флага уведомления MCI.

</dd> <dt>

**вдевицеид**
</dt> <dd>

Идентификатор, возвращенный приложению.

</dd> <dt>

**лпстрдевицетипе**
</dt> <dd>

Имя или идентификатор константы типа устройства. (Обычно имя устройства берется из реестра или файла SYSTEM.INI.) Если этот член является константой, это может быть одно из значений, перечисленных в [типах устройств MCI](mci-device-types.md).

</dd> <dt>

**лпстрелементнаме**
</dt> <dd>

Элемент Device (часто путь).

</dd> <dt>

**лпстралиас**
</dt> <dd>

Необязательный псевдоним устройства.

</dd> </dl>

## <a name="remarks"></a>Remarks

При назначении данных членам этой структуры установите соответствующие флаги в параметре *фдвкомманд* функции [**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85)) , чтобы проверить элементы.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>МЦиапи. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**MCI**](mci.md)
</dt> <dt>

[**Структуры MCI**](mci-structures.md)
</dt> <dt>

[**MCI \_ открыт**](mci-open.md)
</dt> <dt>

[**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85))
</dt> </dl>

 

