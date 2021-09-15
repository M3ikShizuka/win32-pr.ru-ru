---
description: регистрирует службы оболочки платформа динамических данных Exchange (DDE) в текущем процессе, уведомляя систему о том, что текущему процессу требуется разместить объекты DDE.
ms.assetid: d7f65d6a-a697-475b-a739-c7950b7f4d5d
title: Функция Шеллддеинит
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ShellDDEInit
api_type:
- DllExport
api_location:
- Shdocvw.dll
ms.openlocfilehash: cb2f4639d97a99cd063f372e303fd48b7a1d6e4d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460328"
---
# <a name="shellddeinit-function"></a>Функция Шеллддеинит

регистрирует службы оболочки платформа динамических данных Exchange (DDE) в текущем процессе, уведомляя систему о том, что текущему процессу требуется разместить объекты DDE.

## <a name="syntax"></a>Синтаксис


```C++
void ShellDDEInit(
  _In_ BOOL init
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Инициализация* \[ окне\]
</dt> <dd>

Тип: **bool** .

**Значение true** , чтобы зарегистрировать текущий процесс в качестве узла DDE; **Значение false** , чтобы отменить регистрацию.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Remarks

Процесс, вызывающий эту функцию, выступает в качестве оболочки и используется для просмотра содержимого папок, открытых с помощью команды "Open" [**ShellExecute**](/windows/desktop/api/Shellapi/nf-shellapi-shellexecutea) .

Эта функция не имеет связанного заголовка или файла библиотеки, поэтому она должна вызываться по порядковому значению. Вызовите [**LoadLibrary**](/windows/win32/api/libloaderapi/nf-libloaderapi-loadlibrarya) с именем DLL (Shdocvw.dll), чтобы получить маркер модуля. Затем вызовите [**GetProcAddress**](/windows/win32/api/libloaderapi/nf-libloaderapi-getprocaddress) с этим обработчиком модуля и номером функции с порядковым номером 118, чтобы получить адрес функции.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP, Windows 2000 Professional классические \[ приложения\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                          |
| DLL<br/>                      | <dl> <dt>Shdocvw.dll (версия 6,0 или более поздняя)</dt> </dl> |



 

 
