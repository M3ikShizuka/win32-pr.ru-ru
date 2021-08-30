---
description: Регистрируется для уведомления при первой загрузке библиотеки DLL. Это уведомление происходит до того, как будет выполнена динамическая компоновка.
ms.assetid: c2757aa0-76fa-427a-a4f6-cb26e7f7d0d1
title: Функция Лдррегистердллнотификатион
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- LdrRegisterDllNotification
api_type:
- DllExport
api_location:
- ntdll.dll
ms.openlocfilehash: a71798459f487724705b25db019a1f20d77f87ad5a2e4173b47282db062508ce
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120079804"
---
# <a name="ldrregisterdllnotification-function"></a>Функция Лдррегистердллнотификатион

\[эта функция может быть изменена или удалена из Windows без предварительного уведомления.\]

Регистрируется для уведомления при первой загрузке библиотеки DLL. Это уведомление происходит до того, как будет выполнена динамическая компоновка.

## <a name="syntax"></a>Синтаксис


```C++
NTSTATUS NTAPI LdrRegisterDllNotification(
  _In_     ULONG                          Flags,
  _In_     PLDR_DLL_NOTIFICATION_FUNCTION NotificationFunction,
  _In_opt_ PVOID                          Context,
  _Out_    PVOID                          *Cookie
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Флаги* \[ окне\]
</dt> <dd>

Этот параметр должен быть равен нулю.

</dd> <dt>

*Нотификатионфунктион* \[ окне\]
</dt> <dd>

Указатель на функцию обратного вызова уведомления [*лдрдллнотификатион*](ldrdllnotification.md) для вызова при загрузке библиотеки DLL.

</dd> <dt>

*Контекст* \[ в необязательное\]
</dt> <dd>

Указатель на данные контекста для функции обратного вызова.

</dd> <dt>

*Файл cookie* \[ заполняет\]
</dt> <dd>

Указатель на переменную, которая получает идентификатор для функции обратного вызова. Этот идентификатор используется для отмены регистрации функции обратного вызова уведомлений.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если функция завершается успешно, возвращается **состояние \_ Success**.

Формы и значения кодов ошибок **NTSTATUS** перечислены в файле заголовка NTSTATUS. h, доступном в WDK, и описаны в документации по WDK.

## <a name="remarks"></a>Remarks

Эта функция не имеет связанного файла заголовка. Связанная библиотека импорта, NTDLL. lib, доступна в WDK. Можно также использовать функции [**LoadLibrary**](/windows/win32/api/libloaderapi/nf-libloaderapi-loadlibrarya) и [**GetProcAddress**](/windows/win32/api/libloaderapi/nf-libloaderapi-getprocaddress) для динамической привязки к Ntdll.dll.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                 |
| DLL<br/>                      | <dl> <dt>Ntdll.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[*лдрдллнотификатион*](ldrdllnotification.md)
</dt> <dt>

[**лдрунрегистердллнотификатион**](ldrunregisterdllnotification.md)
</dt> </dl>

 

 
