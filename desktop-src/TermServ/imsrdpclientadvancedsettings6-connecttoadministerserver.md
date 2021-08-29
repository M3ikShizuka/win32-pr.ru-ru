---
title: IMsRdpClientAdvancedSettings6 Коннекттоадминистерсервер, свойство
description: возвращает или задает значение, указывающее, должен ли элемент управления ActiveX пытаться подключиться к серверу для административных целей.
ms.assetid: b98f9b9b-a3e7-4a3c-a7e3-e388ce53c5c9
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов свойства Коннекттоадминистерсервер
- Службы удаленных рабочих столов свойства Коннекттоадминистерсервер, интерфейс IMsRdpClientAdvancedSettings6
- Службы удаленных рабочих столов интерфейса IMsRdpClientAdvancedSettings6, свойство Коннекттоадминистерсервер
- Службы удаленных рабочих столов свойства Коннекттоадминистерсервер, интерфейс IMsRdpClientAdvancedSettings7
- Службы удаленных рабочих столов интерфейса IMsRdpClientAdvancedSettings7, свойство Коннекттоадминистерсервер
- Службы удаленных рабочих столов свойства Коннекттоадминистерсервер, интерфейс IMsRdpClientAdvancedSettings8
- Службы удаленных рабочих столов интерфейса IMsRdpClientAdvancedSettings8, свойство Коннекттоадминистерсервер
topic_type:
- apiref
api_name:
- IMsRdpClientAdvancedSettings6.ConnectToAdministerServer
- IMsRdpClientAdvancedSettings6.get_ConnectToAdministerServer
- IMsRdpClientAdvancedSettings6.put_ConnectToAdministerServer
- IMsRdpClientAdvancedSettings7.ConnectToAdministerServer
- IMsRdpClientAdvancedSettings7.get_ConnectToAdministerServer
- IMsRdpClientAdvancedSettings7.put_ConnectToAdministerServer
- IMsRdpClientAdvancedSettings8.ConnectToAdministerServer
- IMsRdpClientAdvancedSettings8.get_ConnectToAdministerServer
- IMsRdpClientAdvancedSettings8.put_ConnectToAdministerServer
api_location:
- MsTscAx.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0a1df4327a263f5bc77fa482e3f84bb971cd5fb047a7c2fed7c1092efdd4d06f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119771674"
---
# <a name="imsrdpclientadvancedsettings6connecttoadministerserver-property"></a>Свойство IMsRdpClientAdvancedSettings6:: Коннекттоадминистерсервер

возвращает или задает значение, указывающее, должен ли элемент управления ActiveX пытаться подключиться к серверу для административных целей.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_ConnectToAdministerServer(
  [in]  VARIANT_BOOL connectToAdministerServer
);

HRESULT get_ConnectToAdministerServer(
  [out] VARIANT_BOOL *pConnectToAdministerServer
);
```



## <a name="property-value"></a>Значение свойства

**Вариант \_ значение TRUE** , чтобы элемент управления ActiveX пытался подключиться к серверу для административных целей. в противном случае значение **\_ false**. Значение по умолчанию — **Variant \_ false**.

## <a name="remarks"></a>Remarks

Чтобы использовать **коннекттоадминистерсервер**, необходимо запустить клиент Подключение К УДАЛЕННОМУ РАБОЧЕМУ столу (RDC) версии 6,1 или более поздней.

> [!Note]  
> RDC версии 6,1 (6.0.6001) поддерживает протокол удаленного рабочего стола 6,1. RDC 6,1 входит в состав Windows Server 2008 и Windows Vista с пакетом обновления 1 (SP1).

 

**Коннекттоадминистерсервер** подключает вас к сеансу, который используется для административных целей на удаленном сервере. Если служба роли узла сеансов удаленный рабочий стол (узел сеансов удаленных рабочих столов) установлена на удаленном сервере, **коннекттоадминистерсервер** выполняет следующие действия:

-   Отключает лицензирование службы удаленных рабочих столов клиентского доступа для сеанса.
-   Отключает перенаправление часового пояса для сеанса.
-   Отключает перенаправление подключение к удаленному рабочему столу Broker (RDCB) для сеанса.
-   Отключает перенаправление устройств самонастраивающийся для сеанса.
-   изменяет тему удаленного сеанса на Windows классической для сеанса.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                         |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                                   |
| Библиотека типов<br/>             | <dl> <dt>MsTscAx.dll</dt> </dl>           |
| DLL<br/>                      | <dl> <dt>MsTscAx.dll</dt> </dl>           |
| IID<br/>                      | IID \_ IMsRdpClientAdvancedSettings6 определен как 222c4b5d-45d9-4df0-a7c6-60cf9089d285<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**IMsRdpClientAdvancedSettings7**](imsrdpclientadvancedsettings7.md)
</dt> <dt>

[**IMsRdpClientAdvancedSettings8**](imsrdpclientadvancedsettings8.md)
</dt> <dt>

[**IMsRdpClientAdvancedSettings6**](imsrdpclientadvancedsettings6.md)
</dt> </dl>

 

 





