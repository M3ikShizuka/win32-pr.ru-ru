---
title: Класс MDM_Policy_Config01_ActiveXControls02
description: этот параметр политики определяет, какие ActiveX сайты установки могут использовать стандартные пользователи в организации для установки ActiveX элементов управления на своих компьютерах.
ms.assetid: 242888ae-f07a-40b7-9539-29fcca9cfc40
keywords:
- Класс MDM_Policy_Config01_ActiveXControls02
- MDM_Policy_Config01_ActiveXControls02 класс, описание
topic_type:
- apiref
api_name:
- MDM_Policy_Config01_ActiveXControls02
- MDM_Policy_Config01_ActiveXControls02.InstanceID
- MDM_Policy_Config01_ActiveXControls02.ParentID
api_location:
- DMWmiBridgeProv.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ef69cd2ad0de4e14b726d5a007273d098a69cd90522c25e5cec640de3f322d8d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120045724"
---
# <a name="mdm_policy_config01_activexcontrols02-class"></a>\_Класс политики MDM \_ Config01 \_ ActiveXControls02

\[Некоторые сведения относятся к предварительно выпущенному продукту, который может быть значительно изменен перед коммерческой выпуском. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, относительно предоставленной здесь информации.\]

этот параметр политики определяет, какие ActiveX сайты установки могут использовать стандартные пользователи в организации для установки ActiveX элементов управления на своих компьютерах. Если этот параметр включен, администратор может создать список утвержденных сайтов установки ActiveX, указанных по URL-адресу узла.

Следующий синтаксис упрощен из MOF-кода и включает все унаследованные свойства.

## <a name="syntax"></a>Синтаксис

``` syntax
[InPartition("local-system"), dynamic, provider("DMWmiBridgeProv")]
class MDM_Policy_Config01_ActiveXControls02
{
  string InstanceID;
  string ParentID;
  string ApprovedInstallationSites;
};
```

## <a name="members"></a>Члены

Класс **\_ политики MDM \_ Config01 \_ ActiveXControls02** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **\_ политики MDM \_ Config01 \_ ActiveXControls02** имеет следующие свойства.

<dl> <dt>

[аппровединсталлатионситес](/windows/client-management/mdm/policy-csp-activexcontrols#activexcontrols-approvedinstallationsites)
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: чтение и запись
</dt> </dl>

</dd> <dt>

**InstanceID**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [ **ключ**](/windows/desktop/WmiSdk/key-qualifier)
</dt> </dl>

</dd> <dt>

**ParentID**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [ **ключ**](/windows/desktop/WmiSdk/key-qualifier)
</dt> </dl>

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10 \[ только классические приложения\]<br/>                                                    |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                      |
| Пространство имен<br/>                | Корневой \\ CIMV2 \\ MDM \\ дммап<br/>                                                             |
| MOF<br/>                      | <dl> <dt>Дмвмибриджепров. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>DMWmiBridgeProv.dll</dt> </dl> |



 

