---
title: Метод Сетпрофилепас класса Win32_TerminalServiceSetting
description: Метод Сетпрофилепас задает свойство filePath для класса.
ms.assetid: a0dfe6a4-929c-45ec-bd31-7e0ffb6ce5de
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Сетпрофилепас
- Службы удаленных рабочих столов метода Сетпрофилепас, класс Win32_TerminalServiceSetting
- Класс Win32_TerminalServiceSetting службы удаленных рабочих столов, метод Сетпрофилепас
topic_type:
- apiref
api_name:
- Win32_TerminalServiceSetting.SetProfilePath
api_location:
- TSCfgWmi.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 434909471accc191e79c92287ab6e4ac427bf949
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967946"
---
# <a name="setprofilepath-method-of-the-win32_terminalservicesetting-class"></a>Метод Сетпрофилепас \_ класса Win32 терминалсервицесеттинг

Метод **сетпрофилепас** задает свойство **FilePath** для класса.

## <a name="syntax"></a>Синтаксис


```mof
uint32 SetProfilePath(
  [in] string ProfilePath
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Путь к пути* \[ окне\]
</dt> <dd>

Новое значение для свойства **FilePath** , которое указывает путь к профилю для компьютера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает успешное завершение, в противном случае возвращает код ошибки WMI. Список этих значений см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md) .

## <a name="remarks"></a>Комментарии

файлы MOF-файл (MOF) содержат определения для классов инструментарий управления Windows (WMI) (WMI). файлы MOF не устанавливаются в составе пакета средств разработки программного обеспечения Microsoft Windows Software Development Kit (SDK). Они устанавливаются на сервере при добавлении связанной роли с помощью диспетчер сервера. Дополнительные сведения о файлах MOF см. в разделе [MOF-файл (MOF)](/windows/desktop/WmiSdk/managed-object-format--mof-).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Пространство имен<br/>                | Корневой \\ CIMv2 \\ терминалсервицес<br/>                                                |
| MOF<br/>                      | <dl> <dt>Тскфгвми. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>TSCfgWmi.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Терминалсервицесеттинг Win32**](win32-terminalservicesetting.md)
</dt> </dl>

 

