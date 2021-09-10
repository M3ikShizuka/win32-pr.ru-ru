---
title: Определение интерфейса, который поддерживает объект
description: Определение интерфейса, который поддерживает объект
ms.assetid: cf2aacb7-5315-4907-a49b-3eb3bbfd13d1
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 066523503232926f5c031efa2cee5ad7a2b05d24
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371691"
---
# <a name="determining-which-interface-an-object-supports"></a>Определение интерфейса, который поддерживает объект

Метод **QueryInterface** позволяет приложению запрашивать объект, чтобы определить, какие интерфейсы он поддерживает. Пример приложения устанавливает указатель *ППВ* на текущий интерфейс.


```C++
STDMETHODIMP CAVIFileCF::QueryInterface( 
    const IID FAR& iid, 
    void FAR* FAR* ppv) 
{ 
    if (iid == IID_IUnknown) 
        *ppv = this;                     // set the interface pointer 
                                         // to this instance 
    else if (iid == IID_IClassFactory) 
        *ppv = this;                     // second chance to set the 
                                         // interface pointer to this 
                                         // instance 
    else 
        return ResultFromScode(E_NOINTERFACE); 
    AddRef();  //Increment the reference count 
    return NULL; 
} 

```



 

 




