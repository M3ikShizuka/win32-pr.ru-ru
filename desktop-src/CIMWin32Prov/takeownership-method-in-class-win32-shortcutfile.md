---
description: Метод Такеовнершип класса Win32_ShortcutFile — Такеовнершип&\# 8194; Метод класса WMI получает владение логическим файлом, указанным в пути объекта.
ms.assetid: 1a8ff156-50b2-4550-abcc-7a6ae0e4630f
ms.tgt_platform: multiple
title: Метод Такеовнершип класса Win32_ShortcutFile
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Win32_ShortcutFile.TakeOwnerShip
api_type:
- COM
api_location:
- CIMWin32.dll
ms.openlocfilehash: 36364a55276842518480c3d3d37c57c3ae0a06ba
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054507"
---
# <a name="takeownership-method-of-the-win32_shortcutfile-class"></a>Метод Такеовнершип \_ класса Win32 шорткутфиле

Метод  [класса WMI](/windows/desktop/WmiSdk/retrieving-a-class) такеовнершип получает владение логическим файлом, указанным в пути объекта. Если логический файл фактически является каталогом, **такеовнершип** работает рекурсивно, перепринимая владение всеми файлами и подкаталогами, которые содержит каталог.

В этом разделе используется синтаксис MOF-файл (MOF). Дополнительные сведения об использовании этого метода см. [в разделе вызов метода](/windows/desktop/WmiSdk/calling-a-method).

## <a name="syntax"></a>Синтаксис


```mof
uint32 TakeOwnerShip();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из следующих целочисленных значений.

<dl> <dt>

**0**
</dt> <dd>

Запрос выполнен успешно.

</dd> <dt>

**2**
</dt> <dd>

Отказано в доступе.

</dd> <dt>

**8**
</dt> <dd>

Произошла неопределенная ошибка.

</dd> <dt>

**9**
</dt> <dd>

Указано недопустимое имя.

</dd> <dt>

**10**
</dt> <dd>

Указанный объект уже существует.

</dd> <dt>

**11**
</dt> <dd>

Файловая система не является системой NTFS.

</dd> <dt>

**12**
</dt> <dd>

Платформа не Windows.

</dd> <dt>

**13**
</dt> <dd>

Диск не совпадает.

</dd> <dt>

**14**
</dt> <dd>

Каталог не пуст.

</dd> <dt>

**15**
</dt> <dd>

Нарушение общего доступа.

</dd> <dt>

**16**
</dt> <dd>

Указан недопустимый файл запуска.

</dd> <dt>

**17**
</dt> <dd>

Привилегия, необходимая для операции, не удерживается.

</dd> <dt>

**открыт**
</dt> <dd>

Указан недопустимый параметр.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Пространство имен<br/>                | Корневой \\ CIMV2<br/>                                                                  |
| MOF<br/>                      | <dl> <dt>CIMWin32. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Классы операционной системы](/previous-versions//aa392727(v=vs.85))
</dt> <dt>

[**\_Шорткутфиле Win32**](win32-shortcutfile.md)
</dt> </dl>

 

