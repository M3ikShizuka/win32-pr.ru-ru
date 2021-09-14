---
description: Метод Коллектусеринфо объекта Installer вызывает последовательность мастера пользовательского интерфейса, которая собирает и сохраняет сведения о пользователе и код продукта.
ms.assetid: 2faacf38-1af1-4e8a-a3f6-87733104614e
title: Метод Installer. Коллектусеринфо
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Installer.CollectUserInfo
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: d7286fdbc9fab6b3db6752284bf86db05f920bd7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171736"
---
# <a name="installercollectuserinfo-method"></a>Метод Installer. Коллектусеринфо

Метод **коллектусеринфо** объекта [**Installer**](installer-object.md) вызывает последовательность мастера пользовательского интерфейса, которая собирает и сохраняет сведения о пользователе и код продукта.

## <a name="syntax"></a>Синтаксис


```JScript
Installer.CollectUserInfo(
  Product
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Продукт* 
</dt> <dd>

Указывает [**код продукта**](productcode.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

Приложение должно вызывать метод **коллектусеринфо** при первом запуске. Метод **коллектусеринфо** открывает пакет установки продукта и вызывает последовательность мастера созданного пользовательского интерфейса, который собирает сведения о пользователе. После завершения последовательности мастера регистрируется собранная информация о пользователе. Свойству [**duilevel**](installer-uilevel.md) должно быть присвоено значение мсиуилевелфулл, так как этот API требует созданного пользовательского интерфейса.

Метод **коллектусеринфо** вызывает [диалоговое окно файла firstrun](firstrun-dialog.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ иинсталлер определен как 000C1090-0000-0000-C000-000000000046<br/>                                                                                                                                                                           |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мсиколлектусеринфо**](/windows/desktop/api/Msi/nf-msi-msicollectuserinfoa)
</dt> </dl>

 

 




