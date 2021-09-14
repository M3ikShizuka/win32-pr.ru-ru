---
title: Метод Тсгстореконсентмсг класса Win32_TSGatewayServerSettings
description: Обновляет сообщение согласия для сервера шлюза.
ms.assetid: b3146d87-95af-4b6b-8c02-5ac4748fbe98
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Тсгстореконсентмсг
- Службы удаленных рабочих столов метода Тсгстореконсентмсг, класс Win32_TSGatewayServerSettings
- Класс Win32_TSGatewayServerSettings службы удаленных рабочих столов, метод Тсгстореконсентмсг
topic_type:
- apiref
api_name:
- Win32_TSGatewayServerSettings.TSGStoreConsentMsg
api_location:
- AagWmi.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 907097739d21e1523aca3b719cdb5f18b6f3fa30
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170603"
---
# <a name="tsgstoreconsentmsg-method-of-the-win32_tsgatewayserversettings-class"></a>Метод Тсгстореконсентмсг \_ класса Win32 тсгатевайсерверсеттингс

Обновляет сообщение согласия для сервера шлюза.

## <a name="syntax"></a>Синтаксис


```mof
uint32 TSGStoreConsentMsg(
  [in] string TSGConMsgText
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Тсгконмсгтекст* \[ окне\]
</dt> <dd>

Тип: **строка**

Текст сообщения согласия.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **UInt32**

Если метод завершается с ошибкой, он возвращает ноль. Если метод завершился неудачно, он возвращает ненулевое значение. Список кодов ошибок см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md).

## <a name="remarks"></a>Remarks

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
</dt> </dl>

 

