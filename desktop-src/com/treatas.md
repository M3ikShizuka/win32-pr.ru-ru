---
title: треатас
description: Указывает идентификатор CLSID класса, который может эмулировать текущий класс.
ms.assetid: 1d7a1677-738a-4258-9afc-e77bd0dcf40f
keywords:
- COM раздела реестра Треатас
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: cf4340b398d6a98b0445cee932da120e23355b71
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369573"
---
# <a name="treatas"></a>треатас

Указывает идентификатор CLSID класса, который может эмулировать текущий класс.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID
   {CLSID}
      TreatAs = {CLSID_TreatAs}
```

## <a name="remarks"></a>Remarks

Это значение **reg \_ SZ** .

Эмуляция — это способность одного приложения открывать и редактировать объект другого класса, сохраняя исходный формат объекта. Разрешение происходит на локальном компьютере, поэтому в случае удаленной активации разрешение происходит на клиентском компьютере с использованием идентификатора CLSID, заданного параметром **треатас**.

DCOM просматривает локальный реестр для **треатас**, даже если вызвать функцию [**CoCreateInstance**](/windows/desktop/api/combaseapi/nf-combaseapi-cocreateinstance) и указать удаленный сервер. Это означает, что если имеется запись **треатас** для класса Class1, которую следует рассматривать как Class2 на локальном компьютере, но вы вызываете **CoCreateInstance** для создания экземпляра Class1 и указываете удаленный сервер, DCOM попытается создать экземпляр класса Class2 на удаленном сервере, даже если Class2 не зарегистрирован на удаленном сервере, что приведет к сбою вызова **CoCreateInstance** .

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[**аутотреатас**](autotreatas.md)
</dt> <dt>

[**кожеттреатаскласс**](/windows/desktop/api/combaseapi/nf-combaseapi-cogettreatasclass)
</dt> <dt>

[**котреатаскласс**](/windows/desktop/api/Objbase/nf-objbase-cotreatasclass)
</dt> </dl>

 

 




