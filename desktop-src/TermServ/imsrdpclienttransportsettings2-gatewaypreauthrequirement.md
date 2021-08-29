---
title: IMsRdpClientTransportSettings2 Гатевайпреаусрекуиремент, свойство
description: Указывает или получает параметр, указывающий, включена ли функция одноразового пароля (OTP) шлюза удаленный рабочий стол.
ms.assetid: cc8f7ebb-16ba-45ed-ba66-de4a339946d0
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов свойства Гатевайпреаусрекуиремент
- Службы удаленных рабочих столов свойства Гатевайпреаусрекуиремент, интерфейс IMsRdpClientTransportSettings2
- Службы удаленных рабочих столов интерфейса IMsRdpClientTransportSettings2, свойство Гатевайпреаусрекуиремент
topic_type:
- apiref
api_name:
- IMsRdpClientTransportSettings2.GatewayPreAuthRequirement
- IMsRdpClientTransportSettings2.get_GatewayPreAuthRequirement
- IMsRdpClientTransportSettings2.put_GatewayPreAuthRequirement
api_location:
- MsTscAx.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 72dd588cd3280128dde654497de359a901182935035213e420831857ab5c9f93
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119771264"
---
# <a name="imsrdpclienttransportsettings2gatewaypreauthrequirement-property"></a>Свойство IMsRdpClientTransportSettings2:: Гатевайпреаусрекуиремент

Указывает или получает параметр, указывающий, включена ли функция одноразового пароля (OTP) шлюза удаленный рабочий стол.

Если включен OTP, **гатевайпреаусрекуиремент** пытается запросить файл cookie OTP из хранилища файлов cookie Интернета с помощью свойства [**гатевайпреауссервераддр**](imsrdpclienttransportsettings2-gatewaypreauthserveraddr.md) . В случае успеха **гатевайпреаусрекуиремент** отправляет файл cookie OTP на сервер брандмауэра (например, Microsoft Internet Security and Acceleration \[ ISA \] Server) для предварительной проверки подлинности.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_GatewayPreAuthRequirement(
  [in]  ULONG ulProxyPreAuthRequirement
);

HRESULT get_GatewayPreAuthRequirement(
  [out] ULONG *pulProxyPreAuthRequirement
);
```



## <a name="property-value"></a>Значение свойства

Если задано значение 1, функция OTP включена. Если задано значение 0, функция OTP отключена.

## <a name="error-codes"></a>Коды ошибок

При успешном выполнении возвращает значение **\_ ОК** .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista с пакетом обновления 1 (SP1)<br/>                                                                 |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                                    |
| Библиотека типов<br/>             | <dl> <dt>MsTscAx.dll</dt> </dl>            |
| DLL<br/>                      | <dl> <dt>MsTscAx.dll</dt> </dl>            |
| IID<br/>                      | IID \_ IMsRdpClientTransportSettings2 определен как 67341688-D606-4c73-A5D2-2E0489009319<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**имсрдпклиенттранспортсеттингс**](imsrdpclienttransportsettings.md)
</dt> <dt>

[**IMsRdpClientTransportSettings2**](imsrdpclienttransportsettings2.md)
</dt> </dl>

 

 





