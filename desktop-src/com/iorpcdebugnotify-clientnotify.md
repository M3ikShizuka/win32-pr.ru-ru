---
title: Иорпкдебугнотифи Клиентнотифи, метод
description: Информирует клиента о том, что исходящий запрос отладчика к серверу.
ms.assetid: a41e3eaa-6d1f-46bf-9103-f83e45b2cd90
keywords:
- COM-метод Клиентнотифи
- Метод Клиентнотифи COM, интерфейс Иорпкдебугнотифи
- Интерфейс Иорпкдебугнотифи COM, метод Клиентнотифи
topic_type:
- apiref
api_name:
- IOrpcDebugNotify.ClientNotify
api_location:
- N/A
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c9e788a51e278df09715aaf9d4993ac5724ed65b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126889096"
---
# <a name="iorpcdebugnotifyclientnotify-method"></a>Метод Иорпкдебугнотифи:: Клиентнотифи

Информирует клиента о том, что исходящий запрос отладчика к серверу.

> [!Note]  
> библиотека импорта, содержащая функцию **клиентнотифи** , не включена в пакет средств разработки программного обеспечения (SDK) Microsoft Windows. Приложение может использовать функции [**GetProcAddress**](/windows/desktop/api/libloaderapi/nf-libloaderapi-getprocaddress) и [**Ошибка GetModuleHandle**](/windows/desktop/api/libloaderapi/nf-libloaderapi-getmodulehandlea) для получения указателя на функцию [**дллдебугобжектрпчук**](dlldebugobjectrpchook.md) из oleaut.dll и предоставления этой функции через интерфейс [**иорпкдебугнотифи**](iorpcdebugnotify.md) .

 

## <a name="syntax"></a>Синтаксис


```C++
void ClientNotify(
   ORPC_DBG_ALL *lpOrpcDebugAll
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*лпорпкдебугалл* 
</dt> <dd>

Указатель на структуру [**ОРПК \_ dbg \_ ALL**](orpc-dbg-all.md) , содержащую сведения об уведомлении, которые система com RPC передает отладчику.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                     |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                           |
| Заголовок<br/>                   | <dl> <dt>Н/Д</dt> </dl> |
| IDL<br/>                      | <dl> <dt>Н/Д</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_аргументы инициализации \_ ОРПК**](orpc-init-args.md)
</dt> <dt>

[**дллдебугобжектрпчук**](dlldebugobjectrpchook.md)
</dt> <dt>

[**иорпкдебугнотифи**](iorpcdebugnotify.md)
</dt> </dl>

 

