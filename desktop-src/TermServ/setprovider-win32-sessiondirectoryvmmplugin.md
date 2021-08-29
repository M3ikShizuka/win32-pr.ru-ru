---
title: Метод Сетпровидер класса Win32_SessionDirectoryVMMPlugin
description: Задает имя поставщика подключаемого модуля.
ms.assetid: fefb7c19-2bab-4ae3-b88b-20da5fd19ff3
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Сетпровидер
- Службы удаленных рабочих столов метода Сетпровидер, класс Win32_SessionDirectoryVMMPlugin
- Класс Win32_SessionDirectoryVMMPlugin службы удаленных рабочих столов, метод Сетпровидер
topic_type:
- apiref
api_name:
- Win32_SessionDirectoryVMMPlugin.SetProvider
api_location:
- TssdWmi.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6a35bccad8421a47e50e6b7a39e7a259852d90af12452056a604f742ad817d36
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119987694"
---
# <a name="setprovider-method-of-the-win32_sessiondirectoryvmmplugin-class"></a>Метод Сетпровидер \_ класса Win32 сессиондиректоривммплугин

Задает имя поставщика подключаемого модуля.

## <a name="syntax"></a>Синтаксис


```mof
uint32 SetProvider(
  [in] string sProvider
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*спровидер* \[ окне\]
</dt> <dd>

Имя поставщика подключаемого модуля.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение 0 при успешном выполнении, в противном случае возвращает код ошибки WMI. Список этих значений см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                              |
| Минимальная версия сервера<br/> | Windows Server 2008 R2<br/>                                                      |
| Пространство имен<br/>                | Корневой \\ CIMv2 \\ терминалсервицес<br/>                                               |
| MOF<br/>                      | <dl> <dt>Тссдвми. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>TssdWmi.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Сессиондиректоривммплугин Win32**](win32-sessiondirectoryvmmplugin.md)
</dt> </dl>

 

 





