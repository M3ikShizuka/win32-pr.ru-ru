---
title: Функция обратного вызова Пксепровидершутдовн
description: Вызывается для завершения работы поставщика.
ms.assetid: 436d7428-18f9-4b73-b346-79c9a0738c31
keywords:
- функция обратного вызова пксепровидершутдовн Windows службах развертывания
topic_type:
- apiref
api_name:
- PxeProviderShutdown
api_type:
- UserDefined
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 5efc7267a5b5e1c15d185b96419210f31981c56c887dd5a8ab7f1068eb4f20ff
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119860794"
---
# <a name="pxeprovidershutdown-callback-function"></a>Функция обратного вызова Пксепровидершутдовн

Вызывается для завершения работы поставщика. Эта функция регистрируется путем вызова функции [**пксерегистеркаллбакк**](/windows/desktop/api/WdsPxe/nf-wdspxe-pxeregistercallback) с параметром *каллбакктипе* , для которого задано **\_ \_ Отключение обратного вызова PXE**. После вызова этой функции обработчик *хпровидер* , переданный функции [*пксепровидеринитиализе*](pxeproviderinitialize.md) , больше не является допустимым.

## <a name="syntax"></a>Синтаксис


```C++
DWORD PXEAPI PxeProviderShutdown(
  _In_ PVOID pContext
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пконтекст* \[ окне\]
</dt> <dd>

Значение контекста, передаваемое функции [**пксерегистеркаллбакк**](/windows/desktop/api/WdsPxe/nf-wdspxe-pxeregistercallback) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если завершение работы поставщика завершается успешно, обратный вызов должен возвращать **ошибку \_ успешно**. В случае сбоя должен возвращаться соответствующий код ошибки.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                          |
| Минимальная версия сервера<br/> | Windows сервер 2008, Windows server 2003 с пакетом обновления 2 (SP2), \[ только классические приложения\]<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Windows Функции сервера служб развертывания](windows-deployment-services-server-functions.md)
</dt> <dt>

[*пксепровидеринитиализе*](pxeproviderinitialize.md)
</dt> <dt>

[**пксерегистеркаллбакк**](/windows/desktop/api/WdsPxe/nf-wdspxe-pxeregistercallback)
</dt> </dl>

 

 





