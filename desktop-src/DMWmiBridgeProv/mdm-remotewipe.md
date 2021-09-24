---
title: Класс MDM_RemoteWipe
description: Класс MDM \_ ремотевипе позволяет выполнять удаленную очистку устройства.
ms.assetid: 8c7c8705-8694-4ce3-ba21-ca610fe1f547
keywords:
- Класс MDM_RemoteWipe
- MDM_RemoteWipe класс, описание
topic_type:
- apiref
api_name:
- MDM_RemoteWipe
- MDM_RemoteWipe.InstanceID
- MDM_RemoteWipe.ParentID
api_location:
- DMWmiBridgeProv.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6ca943ed0b226f9006733b3e9d8745172cfe9e08
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128520061"
---
# <a name="mdm_remotewipe-class"></a>\_Класс MDM ремотевипе

> [!NOTE]
> **Некоторые сведения относятся к предварительной версии продукта, в которую перед коммерческим выпуском могут быть внесены существенные изменения. Корпорация Майкрософт не дает никаких гарантий, явных или подразумеваемых, в отношении предоставленной здесь информации.**

Класс **MDM \_ ремотевипе** позволяет выполнять удаленную очистку устройства.

Следующий пример синтаксиса — упрощенный MOF-код, который включает все наследуемые свойства.

## <a name="syntax"></a>Синтаксис

``` syntax
[InPartition("local-system"), dynamic, provider("DMWmiBridgeProv")]
class MDM_RemoteWipe
{
  string InstanceID;
  string ParentID;
};
```

## <a name="members"></a>Участники

Класс **MDM \_ ремотевипе** имеет следующие типы членов:

-   [Методы](#methods)
-   [Свойства](#properties)

### <a name="methods"></a>Методы

Класс **MDM \_ ремотевипе** содержит следующие методы.

| Метод                                              | Описание                                              |
|:----------------------------------------------------|:---------------------------------------------------------|
| [**довипемесод**](mdm-remotewipe-dowipemethod.md) | Запускает устройство для запуска удаленной очистки. |
| [**довипеперсистпровисионеддатамесод**](mdm-remotewipe-dowipepersistprovisioneddatamethod.md) | Запускает на устройстве резервное копирование данных подготовки в постоянное расположение и выполняет удаленную очистку на устройстве. Сведения, для которых была создана резервная копия, будут восстановлены и применены к устройству при его возобновлении. |
| [**довипеперсистусердатамесод**](mdm-remotewipe-dowipepersistuserdatamethod.md) | Запускает устройство для запуска удаленной очистки при сохранении учетных записей и данных пользователей. |
| [**довипепротектедмесод**](mdm-remotewipe-dowipeprotectedmethod.md) | Запускает устройство для запуска удаленной очистки на устройстве и полностью очищает внутренний диск. В некоторых конфигурациях устройств эта команда может привести к невозможности загрузки устройства. |

### <a name="properties"></a>Свойства

Класс **MDM \_ ремотевипе** имеет следующие свойства.

<dl> <dt>

**InstanceID**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [ **ключ**](/windows/desktop/WmiSdk/key-qualifier)
</dt> </dl>

Определяет имя родительского узла. Для этого класса строка имеет значение "Ремотевипе".

</dd> <dt>

**ParentID**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [ **ключ**](/windows/desktop/WmiSdk/key-qualifier)
</dt> </dl>

Описывает полный путь к родительскому узлу. Для этого класса строка имеет значение "./вендор/мсфт/"

</dd> </dl>

## <a name="example"></a>Пример

В следующем примере показано, как использовать Ремотевипе и вызывать Довипемесод.

> [!Note]  
> Этот пример должен выполняться с правами локального пользователя системы. Для этого скачайте средство PsExec из <https://technet.microsoft.com/sysinternals/bb897553.aspx> `psexec.exe -i -s cmd.exe` командной строки с повышенными правами администратора и запустите ее.

``` syntax
$namespaceName = "root\cimv2\mdm\dmmap"
$className = "MDM_RemoteWipe"
$methodName = "doWipeMethod"

$session = New-CimSession

$params = New-Object Microsoft.Management.Infrastructure.CimMethodParametersCollection
$param = [Microsoft.Management.Infrastructure.CimMethodParameter]::Create("param", "", "String", "In")
$params.Add($param)

try
{
    $instance = Get-CimInstance -Namespace $namespaceName -ClassName $className -Filter "ParentID='./Vendor/MSFT' and InstanceID='RemoteWipe'"
    $session.InvokeMethod($namespaceName, $instance, $methodName, $params)
}
catch [Exception]
{
    write-host $_ | out-string
}
```

## <a name="requirements"></a>Требования

| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------|
| Минимальная версия клиента | Windows 10 \[ только классические приложения\]                                                    |
| Минимальная версия сервера | Ни одна версия не поддерживается                                                                      |
| Пространство имен                | Корневой \\ CIMv2 \\ MDM \\ дммап                                                             |
| MOF                      | <dl> <dt>Дмвмибриджепров. mof</dt> </dl> |
| DLL                      | <dl> <dt>DMWmiBridgeProv.dll</dt> </dl> |

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Использование сценариев PowerShell с WMI Bridge Provider](/windows/client-management/mdm/using-powershell-scripting-with-the-wmi-bridge-provider)
</dt> </dl>
