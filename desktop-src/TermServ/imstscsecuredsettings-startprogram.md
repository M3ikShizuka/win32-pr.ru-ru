---
title: Имстсксекуредсеттингс Стартпрограм, свойство
description: Указывает программу, запускаемую на удаленном сервере при подключении.
ms.assetid: bd2a5ced-468b-48db-ad51-9940577a0310
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов свойства Стартпрограм
- Службы удаленных рабочих столов свойства Стартпрограм, интерфейс Имстсксекуредсеттингс
- Службы удаленных рабочих столов интерфейса Имстсксекуредсеттингс, свойство Стартпрограм
- Службы удаленных рабочих столов свойства Стартпрограм, интерфейс Имсрдпклиентсекуредсеттингс
- Службы удаленных рабочих столов интерфейса Имсрдпклиентсекуредсеттингс, свойство Стартпрограм
topic_type:
- apiref
api_name:
- IMsTscSecuredSettings.StartProgram
- IMsTscSecuredSettings.get_StartProgram
- IMsTscSecuredSettings.put_StartProgram
- IMsRdpClientSecuredSettings.StartProgram
- IMsRdpClientSecuredSettings.get_StartProgram
- IMsRdpClientSecuredSettings.put_StartProgram
api_location:
- MsTscAx.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7e79612855117f48e629e9a06246f3fad922d37f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168700"
---
# <a name="imstscsecuredsettingsstartprogram-property"></a>Свойство Имстсксекуредсеттингс:: Стартпрограм

Указывает программу, запускаемую на удаленном сервере при подключении.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_StartProgram(
  [in]  BSTR newVal
);

HRESULT get_StartProgram(
  [out] BSTR *pStartProgram
);
```



## <a name="property-value"></a>Значение свойства

Имя новой программы запуска. Максимальная длина этой строки равна максимальному **\_ пути**-1 символам.

## <a name="error-codes"></a>Коды ошибок

При успешном выполнении возвращает значение **\_ ОК** .

## <a name="remarks"></a>Remarks

Если значение этого свойства не задано, будет запущена команда оболочки пользователя сеанса. Команда Shell будет считаться из следующего значения реестра на сервере:

**HKey \_ \_** \\ **программное обеспечение** локального компьютера \\ **Microsoft** \\ **Windows NT** \\ **CurrentVersion** \\ **WinLogon** \\ **Shell**

Дополнительные сведения см. в руководстве [по обеспечению безопасности клиента RDP](providing-for-rdp-client-security.md) .

Дополнительные сведения о веб-подключение к удаленному рабочему столу см. в разделе [требования для веб-подключение к удаленному рабочему столу](requirements-for-remote-desktop-web-connection.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                 |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                           |
| Библиотека типов<br/>             | <dl> <dt>MsTscAx.dll</dt> </dl>   |
| DLL<br/>                      | <dl> <dt>MsTscAx.dll</dt> </dl>   |
| IID<br/>                      | IID \_ имстсксекуредсеттингс определен как c9d65442-a0f9-45b2-8f73-d61d2db8cbb6<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**имсрдпклиентсекуредсеттингс**](imsrdpclientsecuredsettings-interface.md)
</dt> <dt>

[**имстсксекуредсеттингс**](imstscsecuredsettings-interface.md)
</dt> </dl>

 

 





