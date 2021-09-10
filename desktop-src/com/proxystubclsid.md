---
title: проксистубклсид
description: Карты идентификатор IID для идентификатора CLSID в 16-разрядных прокси-библиотеках.
ms.assetid: 07e1e9de-e529-496c-b9f7-e7f799089f02
keywords:
- COM-значение реестра Проксистубклсид
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9adfbe319903b2e278be342d169a2e523c952693
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369590"
---
# <a name="proxystubclsid"></a>проксистубклсид

Карты идентификатор IID для идентификатора CLSID в 16-разрядных прокси-библиотеках.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\Interface
   {IID}
      ProxyStubClsid = {CLSID}
```

## <a name="remarks"></a>Remarks

Это значение **reg \_ SZ** , указывающее идентификатор CLSID для IID.

При добавлении интерфейсов необходимо использовать эту запись для их регистрации (16-разрядные системы), чтобы OLE мог найти соответствующий код удаленного взаимодействия для установления межпроцессного взаимодействия.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[**Интерфейс**](interface-key.md)
</dt> <dt>

[**ProxyStubClsid32**](proxystubclsid32.md)
</dt> </dl>

 

 




