---
title: Функция обратного вызова Пксепровидерсервицеконтрол
description: Вызывается, когда служба WDS получает код управления службой.
ms.assetid: 180ddcda-d111-4c81-9177-db99cbf1449f
keywords:
- функция обратного вызова пксепровидерсервицеконтрол Windows службах развертывания
topic_type:
- apiref
api_name:
- PxeProviderServiceControl
api_type:
- UserDefined
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 406152025518a7fb3bb50e0b44fea72bbd17b5cafbc6907912499b70eae1d5cd
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119999594"
---
# <a name="pxeproviderservicecontrol-callback-function"></a>Функция обратного вызова Пксепровидерсервицеконтрол

Вызывается, когда служба WDS получает код управления службой. Эта функция обратного вызова регистрируется путем вызова функции [**пксерегистеркаллбакк**](/windows/desktop/api/WdsPxe/nf-wdspxe-pxeregistercallback) с параметром *каллбакктипе* , установленным в **\_ \_ \_ элемент управления обратного вызова PXE**.

## <a name="syntax"></a>Синтаксис


```C++
DWORD PXEAPI PxeProviderServiceControl(
  _In_ PVOID pContext,
       DWORD dwControl
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пконтекст* \[ окне\]
</dt> <dd>

Значение контекста, передаваемое функции [**пксерегистеркаллбакк**](/windows/desktop/api/WdsPxe/nf-wdspxe-pxeregistercallback) .

</dd> <dt>

*двконтрол* 
</dt> <dd>

Контрольный код. Список возможных значений см. в описании параметра *двконтрол* функции [*хандлерекс*](/windows/desktop/api/winsvc/nc-winsvc-lphandler_function_ex) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если завершение работы поставщика завершается успешно, обратный вызов должен возвращать **ошибку \_ успешно**. В случае сбоя должен возвращаться соответствующий код ошибки.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                          |
| Минимальная версия сервера<br/> | Windows сервер 2008, Windows server 2003 с пакетом обновления 2 (SP2), \[ только классические приложения\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Windows Функции сервера служб развертывания](windows-deployment-services-server-functions.md)
</dt> <dt>

[**пксерегистеркаллбакк**](/windows/desktop/api/WdsPxe/nf-wdspxe-pxeregistercallback)
</dt> </dl>

 

