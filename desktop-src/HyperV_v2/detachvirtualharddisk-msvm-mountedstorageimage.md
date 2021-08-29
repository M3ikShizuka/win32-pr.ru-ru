---
description: Отсоединяет образ подключенного хранилища, связанный с этим классом.
ms.assetid: C3AB0EEE-71FE-4049-90AB-01F5D77E3B97
title: Метод Детачвиртуалхарддиск класса Msvm_MountedStorageImage
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Msvm_MountedStorageImage.DetachVirtualHardDisk
api_type:
- COM
api_location:
- vmms.exe
ms.openlocfilehash: 8ee19316b5e3cbf5440a243df283379b863ecd026b53471b04dfa01ca6731825
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119682564"
---
# <a name="detachvirtualharddisk-method-of-the-msvm_mountedstorageimage-class"></a>Метод Детачвиртуалхарддиск \_ класса Маунтедсторажеимаже мсвм

Отсоединяет образ подключенного хранилища, связанный с этим классом.

## <a name="syntax"></a>Синтаксис


```mof
uint32 DetachVirtualHardDisk();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Тип: **UInt32**

Этот метод может возвращать одно из следующих значений.

<dl> <dt>

**Успешно** (0)
</dt> <dt>

**Сбой** (1)
</dt> </dl>

## <a name="remarks"></a>Remarks

Доступ к классу [**\_ маунтедсторажеимаже мсвм**](msvm-mountedstorageimage.md) может быть ограничен фильтром контроля учетных записей. Дополнительные сведения см. в разделе [Управление учетными записями пользователей и инструментарий WMI](/windows/desktop/WmiSdk/user-account-control-and-wmi).

## <a name="examples"></a>Примеры

В следующем примере C# показано, как отсоединить файл виртуального жесткого диска. Служебные программы, на которые указывают ссылки, можно найти в [общих служебных программах для примеров виртуализации (v2)](common-utilities-for-the-virtualization-samples-v2.md).


```CSharp
public static void DetachVirtualHardDisk(string path)
{
    ManagementScope scope = new ManagementScope(@"root\virtualization\V2", null);

    ManagementClass mountedStorageImageServiceClass = new ManagementClass("Msvm_MountedStorageImage");

    mountedStorageImageServiceClass.Scope = scope;

    using (ManagementObjectCollection collection = mountedStorageImageServiceClass.GetInstances())
    {
        foreach (ManagementObject image in collection)
        {
            using (image)
            {
                string name = image.GetPropertyValue("Name").ToString();
                if (string.Equals(name, path, StringComparison.OrdinalIgnoreCase))
                {
                    ManagementBaseObject outParams = image.InvokeMethod("DetachVirtualHardDisk", null, null);

                    if ((UInt32)outParams["ReturnValue"] == 0)
                    {
                        Console.WriteLine("{0} was detached successfully.", path);
                    }
                    else
                    {
                        Console.WriteLine("Unable to dettach {0}", path);
                    }

                    outParams.Dispose();

                    break;
                }

                image.Dispose();
            }
        }
    }
}
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                                              |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                                    |
| Пространство имен<br/>                | Корневая \\ виртуализация \\ версии 2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Мсвм \_ маунтедсторажеимаже**](msvm-mountedstorageimage.md)
</dt> </dl>

 

