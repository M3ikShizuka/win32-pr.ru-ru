---
description: Указывает окну IME для получения расположения окна композиции. Чтобы отправить эту команду, приложение использует \_ \_ управляющее сообщение WM IME с параметрами параметров, приведенными ниже.
ms.assetid: d2c60974-a602-4a42-8a45-870ee39df001
title: Команда IMC_GETCOMPOSITIONWINDOW (IMM. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9dc32c183377967071b5f0cdea278a37a414a7eead422a5ed00750174a6667bc
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119068094"
---
# <a name="imc_getcompositionwindow-command"></a>ИМК \_ жеткомпоситионвиндов, команда

Указывает окну IME для получения расположения окна композиции. Чтобы отправить эту команду, приложение использует [**\_ \_ управляющее сообщение WM IME**](wm-ime-control.md) с параметрами параметров, приведенными ниже.


```C++
LRESULT IMC_GETCOMPOSITIONWINDOW
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="wParam"></span><span id="wparam"></span><span id="WPARAM"></span>*wParam*
</dt> <dd>

Задайте для параметра значение ИМК \_ жеткомпоситионвиндов.

</dd> <dt>

<span id="lParam"></span><span id="lparam"></span><span id="LPARAM"></span>*lParam*
</dt> <dd>

Указатель на структуру [**компоситионформ**](/windows/win32/api/imm/ns-imm-compositionform) , содержащую расположение окна композиции.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает 0 в случае успеха или ненулевое значение в противном случае.

## <a name="remarks"></a>Remarks

Так как редактор IME может скорректировать расположение окна композиции, приложение использует эту команду для получения фактического расположения, чтобы решить, следует ли изменить расположение окна. Полученное расположение находится в координатах окна относительно окна, имеющего текущий фокус ввода.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                 |
| Заголовок<br/>                   | <dl> <dt>Imm. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Диспетчер метода ввода](input-method-manager.md)
</dt> <dt>

[Команды диспетчера методов ввода](input-method-manager-commands.md)
</dt> <dt>

[**компоситионформ**](/windows/win32/api/imm/ns-imm-compositionform)
</dt> </dl>

 

 




