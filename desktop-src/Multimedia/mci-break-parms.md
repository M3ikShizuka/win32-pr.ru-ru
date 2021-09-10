---
title: Структура MCI_BREAK_PARMS (МЦиапи. h)
description: '\_Структура пармс разрывов MCI \_ содержит код виртуального ключа и сведения о окне для команды MCI \_ break.'
ms.assetid: c8df8c55-cc6b-4dd7-b275-784d3eb9dce1
keywords:
- структура MCI_BREAK_PARMS Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_BREAK_PARMS
api_location:
- mciapi.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e66b52992827b447b6d4b5585ca3f98564142680
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369898"
---
# <a name="mci_break_parms-structure"></a>\_Структура MCI Break \_ пармс

Структура **\_ \_ Пармс разрывов MCI** содержит код виртуального ключа и сведения о окне для команды [**MCI \_ break**](mci-break.md) .

## <a name="syntax"></a>Синтаксис


```C++
typedef struct {
  DWORD_PTR dwCallback;
  int       nVirtKey;
  HWND      hwndBreak;
} MCI_BREAK_PARMS;
```



## <a name="members"></a>Участники

<dl> <dt>

**двкаллбакк**
</dt> <dd>

Слово нижнего порядка задает маркер окна, используемый для \_ флага уведомления MCI.

</dd> <dt>

**нвирткэй**
</dt> <dd>

Код виртуального ключа для ключа разрыва.

</dd> <dt>

**хвндбреак**
</dt> <dd>

Обработчик для окна, который должен быть текущим окном для обнаружения прерываний.

</dd> </dl>

## <a name="remarks"></a>Remarks

При назначении данных членам этой структуры установите соответствующие флаги в параметре *фдвкомманд* функции [**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85)) , чтобы проверить элементы. Определены следующие флаги:

\_HWND разрыва MCI \_

Проверяет элемент **хвндбреак** , указывающий окно, которое должно иметь фокус на включение обнаружения прерываний.

\_ключ разрыва MCI \_

Проверяет элемент **нвирткэй** , указывающий на код виртуального ключа, который будет использоваться для ключа разрыва.

\_разрыв MCI \_ отключен

Отключает любой существующий ключ разрыва.

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

[**\_разрыв MCI**](mci-break.md)
</dt> <dt>

[**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85))
</dt> </dl>

 

