---
description: отключает возможность закрепления ярлыка или окна на панели задач или в меню. это свойство также делает элемент недоступным для включения в список наиболее часто используемых программных меню.
ms.assetid: 86239BF8-BCFC-4e76-BF94-5ABA4639562C
title: System. Аппусермодел. Превентпиннинг
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7804c615bcb35909610b06622bd25fe3dccdd0f3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127262939"
---
# <a name="systemappusermodelpreventpinning"></a>System. Аппусермодел. Превентпиннинг

Отключает возможность закрепления ярлыка или окна на панели задач или в меню " **Пуск** ". Это свойство также делает элемент недоступным для включения в список наиболее часто используемых программных элементов меню " **Пуск** ".

Это свойство должно быть установлено в окне перед свойством [ \_ \_ идентификатора PKEY аппусермодел](./props-system-appusermodel-id.md) . После \_ \_ установки свойства аппусермодел ID для PKEY изменения в [PKEY \_ аппусермодел \_ превентпиннинг]() игнорируются.

Дополнительные сведения о идентификаторах моделей пользователей приложений (Аппусермоделидс) и других способах исключения элемента из панели задач и о включении часто используемых элементов см. в разделе [идентификаторы моделей пользователей приложений (аппусермоделидс)](../shell/appids.md).

Чтобы задать это свойство в окне, используйте [**шжетпропертисторефорвиндов**](/windows/desktop/api/Shellapi/nf-shellapi-shgetpropertystoreforwindow) для получения хранилища свойств окна и используйте методы, извлекают объект [**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore) , чтобы установить свойство [System. аппусермодел. превентпиннинг]() этого окна.

Установка этого свойства приводит к игнорированию следующих свойств:

-   [System. Аппусермодел. Релаунчкомманд](./props-system-appusermodel-relaunchcommand.md)
-   [System. Аппусермодел. Релаунчдисплайнамересаурце](./props-system-appusermodel-relaunchdisplaynameresource.md)
-   [System. Аппусермодел. Релаунчиконресаурце](./props-system-appusermodel-relaunchiconresource.md)

## <a name="windows-10-version-1703-windows-10-version-1607-windows-10-version-1511-windows-10-version-1507-windows-81-windows-8-windows-7"></a>Windows 10, версия 1703, Windows 10, версия 1607, Windows 10, версия 1511, Windows 10, версия 1507, Windows 8.1, Windows 8, Windows 7

```
propertyDescription
   name = System.AppUserModel.PreventPinning
   shellPKey = PKEY_AppUserModel_PreventPinning
   formatID = 9F4C2855-9F79-4B39-A8D0-E1D42DE1D5F3
   propID = 9
   SearchInfo
      InInvertedIndex = false
      IsColumn = false
   typeInfo
      type = Boolean
      IsInnate = false
```

## <a name="remarks"></a>Remarks

Значения PKEY определены в списке PKEY. h.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Идентификаторы модели пользователя приложения (Аппусермоделидс)](../shell/appids.md)
</dt> <dt>

[System.AppUserModel.ID](./props-system-appusermodel-id.md)
</dt> <dt>

[**шжетпропертисторефорвиндов**](/windows/desktop/api/Shellapi/nf-shellapi-shgetpropertystoreforwindow)
</dt> <dt>

[пропертидескриптионлист](./propdesc-schema-propertydescriptionlist.md)
</dt> <dt>

[пропертидескриптион](./propdesc-schema-propertydescription.md)
</dt> <dt>

[сеарчинфо](./propdesc-schema-searchinfo.md)
</dt> <dt>

[лабелинфо](./propdesc-schema-labelinfo.md)
</dt> <dt>

[typeInfo](./propdesc-schema-typeinfo.md)
</dt> <dt>

[displayInfo](./propdesc-schema-displayinfo.md)
</dt> <dt>

[aliasInfo](./propdesc-schema-aliasinfo.md)
</dt> <dt>

[stringFormat](./propdesc-schema-stringformat.md)
</dt> <dt>

[булеанформат](./propdesc-schema-booleanformat.md)
</dt> <dt>

[numberFormat](./propdesc-schema-numberformat.md)
</dt> <dt>

[dateTimeFormat](./propdesc-schema-datetimeformat.md)
</dt> <dt>

[енумератедлист](./propdesc-schema-enumeratedlist.md)
</dt> <dt>

[enum](./propdesc-schema-enum.md)
</dt> <dt>

[енумранже](./propdesc-schema-enumrange.md)
</dt> <dt>

[image](./propdesc-schema-image.md)
</dt> <dt>

[дравконтрол](./propdesc-schema-drawcontrol.md)
</dt> <dt>

[едитконтрол](./propdesc-schema-editcontrol.md)
</dt> <dt>

[филтерконтрол](./propdesc-schema-filtercontrol.md)
</dt> <dt>

[куериконтрол](./propdesc-schema-querycontrol.md)
</dt> <dt>

[релатедпропертинфо](./propdesc-schema-relatedpropertyinfo.md)
</dt> <dt>

[relatedProperty](./propdesc-schema-relatedproperty.md)
</dt> </dl>

 

 
