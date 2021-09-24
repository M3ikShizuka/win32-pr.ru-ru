---
title: метод Довипепротектедмесод класса MDM_RemoteWipe
description: Запускает устройство для запуска удаленной очистки на устройстве и полностью очищает внутренний диск. В некоторых конфигурациях устройств эта команда может привести к невозможности загрузки устройства.
keywords:
- метод Довипепротектедмесод
- метод Довипепротектедмесод, класс MDM_RemoteWipe
- Класс MDM_RemoteWipe, метод Довипепротектедмесод
topic_type:
- apiref
api_name:
- MDM_RemoteWipe.doWipeProtectedMethod
api_location:
- DMWmiBridgeProv.dll
api_type:
- COM
ms.topic: reference
ms.date: 09/17/2021
ms.openlocfilehash: 792d4e412b8a16869bbfa33229abe541be1c952e
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128523863"
---
# <a name="dowipeprotectedmethod-method-of-the-mdm_remotewipe-class"></a>метод Довипепротектедмесод класса MDM_RemoteWipe

> [!NOTE]
> **Некоторые сведения относятся к предварительной версии продукта, в которую перед коммерческим выпуском могут быть внесены существенные изменения. Корпорация Майкрософт не дает никаких гарантий, явных или подразумеваемых, в отношении предоставленной здесь информации.**

Запускает устройство для запуска удаленной очистки на устройстве и полностью очищает внутренний диск. В некоторых конфигурациях устройств эта команда может привести к невозможности загрузки устройства. См. также [довипеперсистпровисионеддатамесод](/windows/client-management/mdm/remotewipe-csp).

## <a name="syntax"></a>Синтаксис

```mof
uint32 doWipeProtectedMethod(
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
