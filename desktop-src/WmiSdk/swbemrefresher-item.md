---
description: Метод Свбемрефрешер. Item возвращает указанный Свбемрефрешаблеитем из коллекции. Свбемрефрешаблеитем из коллекции.
ms.assetid: 8ae3dea5-0582-422e-9cd8-b6d91b41588a
ms.tgt_platform: multiple
title: Метод Свбемрефрешер. Item (Wbemdisp. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SWbemRefresher.Item
- ISWbemRefresher.Item
- ISWbemRefresher.Item
api_type:
- COM
api_location:
- Wbemdisp.dll
ms.openlocfilehash: 1290a395b9fc3f4e485a90822103ccb51b40edcc1b72fdf08433eaed72cdd213
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119897574"
---
# <a name="swbemrefresheritem-method"></a>Свбемрефрешер. Item, метод

Метод **свбемрефрешер. Item** Возвращает указанный [**свбемрефрешаблеитем**](swbemrefreshableitem.md) из коллекции.

Описание этого синтаксиса см. в разделе [соглашения о документе для API скриптов](document-conventions-for-the-scripting-api.md).

## <a name="syntax"></a>Синтаксис


```VB
objItem = .Item( _
  ByVal lIndex _
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*линдекс* 
</dt> <dd>

Значение индекса элемента в коллекции.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если вызов выполнен успешно, возвращается указанный объект [**свбемрефрешаблеитем**](swbemrefreshableitem.md) .

## <a name="error-codes"></a>Коды ошибок

Если у Обновитель нет элемента с указанным индексом, **вбемеррнотфаунд** создается.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Wbemdisp. h</dt> </dl>   |
| Библиотека типов<br/>             | <dl> <dt>Wbemdisp. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Wbemdisp.dll</dt> </dl> |
| CLSID<br/>                    | \_СВБЕМРЕФРЕШЕР CLSID<br/>                                                        |
| IID<br/>                      | IID \_ исвбемрефрешер<br/>                                                         |



## <a name="see-also"></a>См. также

<dl> <dt>

[**свбемрефрешер**](swbemrefresher.md)
</dt> </dl>

 

 




