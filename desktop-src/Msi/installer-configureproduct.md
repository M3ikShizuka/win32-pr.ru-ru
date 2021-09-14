---
description: Метод Конфигурепродукт объекта Installer устанавливает или удаляет продукт.
ms.assetid: 1215a03f-6c96-4416-881f-0071c1b3c5df
title: Метод Installer. Конфигурепродукт
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Installer.ConfigureProduct
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 989855508215b2cd5d04bff7903628513314b9a5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171699"
---
# <a name="installerconfigureproduct-method"></a>Метод Installer. Конфигурепродукт

Метод **конфигурепродукт** объекта [**Installer**](installer-object.md) устанавливает или удаляет продукт.

## <a name="syntax"></a>Синтаксис


```JScript
Installer.ConfigureProduct(
  Product,
  InstallLevel,
  InstallState
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Продукт* 
</dt> <dd>

Указывает код продукта.

</dd> <dt>

*инсталллевел* 
</dt> <dd>

Задает конфигурацию установки по умолчанию для продукта. Параметр Инсталллевел игнорируется, и все компоненты устанавливаются, если параметру InstallState задано любое другое значение, отличное от Мсиинсталлстатедефаулт.

Для установки подмножества доступных компонентов этот параметр должен быть равен 0 (установить с использованием уровней автора), 65535 (установка всех компонентов) или значение от 0 до 65535.

</dd> <dt>

*InstallState* 
</dt> <dd>

Указывает состояние установки для компонента. Этот параметр должен иметь одно из следующих значений.



| Значение                                                                                                                                                                                                                                        | Значение                                                      |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------|
| <span id="msiInstallStateAdvertised"></span><span id="msiinstallstateadvertised"></span><span id="MSIINSTALLSTATEADVERTISED"></span><dl> <dt>**мсиинсталлстатеадвертисед**</dt> </dl> | Эта функция объявлена<br/>                         |
| <span id="msiInstallStateLocal"></span><span id="msiinstallstatelocal"></span><span id="MSIINSTALLSTATELOCAL"></span><dl> <dt>**мсиинсталлстателокал**</dt> </dl>                     | Этот компонент устанавливается локально.<br/>                 |
| <span id="msiInstallStateAbsent"></span><span id="msiinstallstateabsent"></span><span id="MSIINSTALLSTATEABSENT"></span><dl> <dt>**мсиинсталлстатеабсент**</dt> </dl>                 | Компонент удален.<br/>                       |
| <span id="msiInstallStateSource"></span><span id="msiinstallstatesource"></span><span id="MSIINSTALLSTATESOURCE"></span><dl> <dt>**мсиинсталлстатесаурце**</dt> </dl>                 | Компонент устанавливается для запуска из источника.<br/>      |
| <span id="msiInstallStateDefault"></span><span id="msiinstallstatedefault"></span><span id="MSIINSTALLSTATEDEFAULT"></span><dl> <dt>**мсиинсталлстатедефаулт**</dt> </dl>             | Компонент устанавливается в расположение по умолчанию.<br/> |



 

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

Метод **конфигурепродукт** отображает пользовательский интерфейс, используя текущие параметры. Параметры пользовательского интерфейса можно изменить, изменив [**свойство duilevel (объект установщика)**](installer-uilevel.md) перед вызовом метода **конфигурепродукт** .

Если для параметра *InstallState* задано любое другое значение, отличное от мсиинсталлстатедефаулт, то параметр *инсталллевел* игнорируется и устанавливаются все компоненты продукта. Используйте метод [**конфигурефеатуре**](installer-configurefeature.md) для управления установкой отдельных компонентов, если для параметра *InstallState* не задано значение мсиинсталлстатедефаулт.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ иинсталлер определен как 000C1090-0000-0000-C000-000000000046<br/>                                                                                                                                                                           |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мсиконфигурепродукт**](/windows/desktop/api/Msi/nf-msi-msiconfigureproducta)
</dt> <dt>

[Функции установки и настройки](installer-function-reference.md)
</dt> </dl>

 

 




