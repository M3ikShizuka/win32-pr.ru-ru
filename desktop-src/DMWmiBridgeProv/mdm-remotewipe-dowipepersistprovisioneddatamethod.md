---
title: метод Довипеперсистпровисионеддатамесод класса MDM_RemoteWipe
description: Запускает на устройстве резервное копирование данных подготовки в постоянное расположение и выполняет удаленную очистку на устройстве. Сведения, для которых была создана резервная копия, будут восстановлены и применены к устройству при его возобновлении.
keywords:
- метод Довипеперсистпровисионеддатамесод
- метод Довипеперсистпровисионеддатамесод, класс MDM_RemoteWipe
- Класс MDM_RemoteWipe, метод Довипеперсистпровисионеддатамесод
topic_type:
- apiref
api_name:
- MDM_RemoteWipe.doWipePersistProvisionedDataMethod
api_location:
- DMWmiBridgeProv.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1f346b520499c6a6d0eb5c181f8fd9b5dcd0208b
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128523864"
---
# <a name="dowipepersistprovisioneddatamethod-method-of-the-mdm_remotewipe-class"></a>метод Довипеперсистпровисионеддатамесод класса MDM_RemoteWipe

> [!NOTE]
> **Некоторые сведения относятся к предварительно выпущенному продукту, который может быть значительно изменен перед коммерческой выпуском. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, относительно предоставленной здесь информации.** 
 ![ Эскиз](https://user-images.githubusercontent.com/31261191/133865694-1fae8e8b-c3ba-41a9-bcba-dbb67a6e2130.png)

Запускает на устройстве резервное копирование данных подготовки в постоянное расположение и выполняет удаленную очистку на устройстве. Сведения, для которых была создана резервная копия, будут восстановлены и применены к устройству при его возобновлении. См. также [довипеперсистпровисионеддатамесод](/windows/client-management/mdm/remotewipe-csp).

## <a name="syntax"></a>Синтаксис

```mof
uint32 doWipePersistProvisionedDataMethod(
  [in] string param
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*параметр* \[ окне\]
</dt> <dd></dd> </dl>

## <a name="requirements"></a>Требования

| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10 \[ только классические приложения\]<br/>                                                    |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                      |
| Пространство имен<br/>                | Корневой \\ CIMv2 \\ MDM \\ дммап<br/>                                                             |
| MOF<br/>                      | <dl> <dt>Дмвмибриджепров. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>DMWmiBridgeProv.dll</dt> </dl> |

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_РЕМОТЕВИПЕ MDM**](mdm-remotewipe.md)
</dt> <dt>

[Использование сценариев PowerShell с WMI Bridge Provider](/windows/client-management/mdm/using-powershell-scripting-with-the-wmi-bridge-provider)
</dt> </dl>
