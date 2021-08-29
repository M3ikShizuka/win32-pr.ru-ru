---
description: Связывает бутсаурцесеттингдата Мсвм \_ с общей мсвм \_ виртуалсистемсеттингдата.
ms.assetid: DB2E66F1-CC2C-49FC-96CE-D9DE441AA809
title: Класс Msvm_BootSourceComponent
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Msvm_BootSourceComponent
- Msvm_BootSourceComponent.GroupComponent
- Msvm_BootSourceComponent.PartComponent
api_type:
- DllExport
api_location:
- vmms.exe
ms.openlocfilehash: 44b4b1bb6908a304ddef67d4988069c6fa018235c2d0488179d87e332f6d45e2
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119252964"
---
# <a name="msvm_bootsourcecomponent-class"></a>\_Класс мсвм бутсаурцекомпонент

Связывает [**\_ бутсаурцесеттингдата мсвм**](msvm-bootsourcesettingdata.md) с общей [**мсвм \_ виртуалсистемсеттингдата**](msvm-virtualsystemsettingdata.md). Этот класс является производным [**от \_ компонента CIM**](/windows/desktop/CIMWin32Prov/cim-component).

Следующий синтаксис упрощен из MOF-кода и включает все унаследованные свойства.

## <a name="syntax"></a>Синтаксис

``` syntax
[Association, Dynamic, Provider("VmmsWmiInstanceAndMethodProvider"), AMENDMENT]
class Msvm_BootSourceComponent : CIM_Component
{
  CIM_ManagedSystemElement REF GroupComponent;
  CIM_ManagedSystemElement REF PartComponent;
};
```

## <a name="members"></a>Члены

Класс **мсвм \_ бутсаурцекомпонент** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **мсвм \_ бутсаурцекомпонент** имеет следующие свойства.

<dl> <dt>

**Ссылка**
</dt> <dd> <dl> <dt>

Тип данных: **CIM \_ манажедсистемелемент**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Ссылка на родительский элемент в ассоциации. Это свойство наследуется [**от \_ компонента CIM**](cim-component.md).

</dd> <dt>

**PartComponent**
</dt> <dd> <dl> <dt>

Тип данных: **CIM \_ манажедсистемелемент**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Ссылка на дочерний элемент в ассоциации. Это свойство наследуется [**от \_ компонента CIM**](cim-component.md).

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                                                 |
| Пространство имен<br/>                | Корневая \\ виртуализация \\ версии 2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Компонент CIM**](cim-component.md)
</dt> <dt>

[**\_Компонент CIM**](/windows/desktop/CIMWin32Prov/cim-component)
</dt> <dt>

[**Мсвм \_ бутсаурцесеттингдата**](msvm-bootsourcesettingdata.md)
</dt> <dt>

[**Мсвм \_ виртуалсистемсеттингдата**](msvm-virtualsystemsettingdata.md)
</dt> </dl>

 

