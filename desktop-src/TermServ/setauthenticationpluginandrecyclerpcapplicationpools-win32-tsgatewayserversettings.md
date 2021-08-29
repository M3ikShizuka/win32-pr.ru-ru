---
title: Метод Сетаусентикатионплугинандрециклерпкаппликатионпулс класса Win32_TSGatewayServerSettings
description: Задает текущий подключаемый модуль проверки подлинности для сервера шлюза удаленный рабочий стол шлюза и перезапускает пулы приложений RPC в службах IIS.
ms.assetid: cdceaf50-3d0a-4af0-9ad5-fb43760fcf7b
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Сетаусентикатионплугинандрециклерпкаппликатионпулс
- Службы удаленных рабочих столов метода Сетаусентикатионплугинандрециклерпкаппликатионпулс, класс Win32_TSGatewayServerSettings
- Класс Win32_TSGatewayServerSettings службы удаленных рабочих столов, метод Сетаусентикатионплугинандрециклерпкаппликатионпулс
topic_type:
- apiref
api_name:
- Win32_TSGatewayServerSettings.SetAuthenticationPluginAndRecycleRpcApplicationPools
api_location:
- AagWmi.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a839f13069b296385264b8173b2e7f4a39d47fa190e826e226d1bfa407acaeb5
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119138017"
---
# <a name="setauthenticationpluginandrecyclerpcapplicationpools-method-of-the-win32_tsgatewayserversettings-class"></a>Метод Сетаусентикатионплугинандрециклерпкаппликатионпулс \_ класса Win32 тсгатевайсерверсеттингс

Задает текущий подключаемый модуль проверки подлинности для сервера шлюза удаленный рабочий стол шлюза и перезапускает пулы приложений RPC в службах IIS.

Этот метод эквивалентен вызову методов [**сетаусентикатионплугин**](setauthenticationplugin-win32-tsgatewayserversettings.md) и [**рециклерпкаппликатионпулс**](recyclerpcapplicationpools-win32-tsgatewayserversettings.md) последовательно.

## <a name="syntax"></a>Синтаксис


```mof
uint32 SetAuthenticationPluginAndRecycleRpcApplicationPools(
  [in] string PluginName
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*PluginName* \[ окне\]
</dt> <dd>

Тип: **строка**

Имя подключаемого модуля проверки подлинности

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **UInt32**

Если метод завершается с ошибкой, он возвращает ноль. Если метод завершился неудачно, он возвращает ненулевое значение. Список кодов ошибок см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md).

## <a name="remarks"></a>Remarks

Вызов этого метода приводит к отключению всех существующих подключений.

Для вызова этого метода необходимо быть членом группы администраторов.

файлы MOF-файл (MOF) содержат определения для классов инструментарий управления Windows (WMI) (WMI). файлы MOF не устанавливаются в составе пакета средств разработки программного обеспечения Microsoft Windows Software Development Kit (SDK). Они устанавливаются на сервере при добавлении связанной роли с помощью диспетчер сервера. Дополнительные сведения о файлах MOF см. в разделе [MOF-файл (MOF)](/windows/desktop/WmiSdk/managed-object-format--mof-).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008 R2<br/>                                                        |
| Пространство имен<br/>                | Корневой \\ CIMv2 \\ терминалсервицес<br/>                                                 |
| MOF<br/>                      | <dl> <dt>TSGateway. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>AagWmi.dll</dt> </dl>    |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Тсгатевайсерверсеттингс Win32**](win32-tsgatewayserversettings.md)
</dt> <dt>

[**сетаусентикатионплугин**](setauthenticationplugin-win32-tsgatewayserversettings.md)
</dt> <dt>

[**рециклерпкаппликатионпулс**](recyclerpcapplicationpools-win32-tsgatewayserversettings.md)
</dt> </dl>

 

