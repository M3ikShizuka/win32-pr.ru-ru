---
description: Сетдатетиме&\# 8194; Метод класса WMI задает текущее системное время на компьютере.
ms.assetid: b9b86a52-c3d7-489d-8632-b297970dbeac
ms.tgt_platform: multiple
title: Метод Сетдатетиме класса Win32_OperatingSystem
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Win32_OperatingSystem.SetDateTime
api_type:
- COM
api_location:
- CIMWin32.dll
ms.openlocfilehash: bbab7d9e599fb33fe999ac56eaba5f180895f7658d718cd524bc9685109ae2af
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119760144"
---
# <a name="setdatetime-method-of-the-win32_operatingsystem-class"></a>Метод Сетдатетиме \_ класса операционной системы Win32

Метод  [класса WMI](/windows/desktop/WmiSdk/retrieving-a-class) сетдатетиме задает текущее системное время на компьютере.

В этом разделе используется синтаксис MOF-файл (MOF). Дополнительные сведения об использовании этого метода см. [в разделе вызов метода](/windows/desktop/WmiSdk/calling-a-method).

## <a name="syntax"></a>Синтаксис


```mof
uint32 SetDateTime(
  [in] datetime LocalDatetime
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*LocalDatetime* \[ окне\]
</dt> <dd>

Значение текущего времени.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ноль (0), чтобы указать на успешное выполнение. Любое другое значение указывает на ошибку. Коды ошибок см. в разделе [**константы WMI Error**](/windows/desktop/WmiSdk/wmi-error-constants) или [**вбемерроренум**](/windows/desktop/api/wbemdisp/ne-wbemdisp-wbemerrorenum). Общие значения **HRESULT** см. в разделе [коды системных ошибок](/windows/desktop/Debug/system-error-codes).

<dl> <dt>

**Успешно** (0)
</dt> <dt>

**Другие** (1 4294967295)
</dt> </dl>

## <a name="remarks"></a>Remarks

вызывающий процесс должен иметь \_ \_ привилегию SE SYSTEMTIME NAME.

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

[**Win32, \_ Операционная система**](win32-operatingsystem.md)
</dt> <dt>

[Задачи WMI: управление рабочим столом](/windows/desktop/WmiSdk/wmi-tasks--desktop-management)
</dt> </dl>

 

