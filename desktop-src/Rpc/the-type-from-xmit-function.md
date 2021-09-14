---
title: Функция type_from_xmit
description: Заглушки вызывают тип \_ из \_ функции xmit для преобразования данных из переданного типа в тип, представленный для приложения.
ms.assetid: 679a2738-a166-4e73-bca7-950f979ed97a
keywords:
- type_from_xmit
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e594e8586522dd3697f5ae62c95851917741f73c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127250504"
---
# <a name="the-type_from_xmit-function"></a>Тип \_ из \_ функции xmit

Заглушки вызывают **тип \_ из функции \_ xmit** для преобразования данных из переданного типа в тип, представленный для приложения. Функция определяется следующим образом:

``` syntax
void __RPC_USER <type>_from_xmit ( 
    <xmit_type> __RPC_FAR *, 
    <type> __RPC_FAR *);
```

Первый параметр — это указатель на передаваемые данные. Функция задает второй параметр, указывающий на представленные данные.

**Тип \_ из функции \_ xmit** должен управлять памятью для представляемого типа. Функция должна выделить память для всей структуры данных, которая начинается с адреса, указанного вторым параметром, за исключением самого параметра (заглушка выделяет память для корневого узла и передает ее в функцию). Значение второго параметра не может измениться во время вызова. Функция может изменить содержимое по этому адресу.

В этом примере тип двойной ссылки функции \_ \_ \_ из \_ xmit преобразует массив размеров в список с двойным связыванием. Функция удерживает допустимый указатель на начало списка, освобождает память, связанную с остальной частью списка, а затем создает новый список, который начинается с того же указателя. Функция использует служебную функцию **инсертневноде** для добавления узла списка в конец списка и назначения указателей *пнекст* и *ппревиаус* соответствующим значениям.


```C++
void __RPC_USER DOUBLE_LINK_TYPE_from_xmit(
     DOUBLE_XMIT_TYPE __RPC_FAR * pArray,
     DOUBLE_LINK_TYPE __RPC_FAR * pList)
{
    DOUBLE_LINK_TYPE *pCurrent;
    int i;
 
    if (pArray->sSize <= 0) 
    {  
        // error checking
        return;
    }
 
    if (pList == NULL) // if invalid, create the list head
        pList = InsertNewNode(pArray->asNumber[0], NULL);             
    else 
    {    
        DOUBLE_LINK_TYPE_free_inst(pList);  // free all other nodes
        pList->sNumber = pArray->asNumber[0];
        pList->pNext = NULL; 
    }
 
    pCurrent = pList; 
    for (i = 1; i < pArray->sSize; i++)  
        pCurrent = InsertNewNode(pArray->asNumber[i], pCurrent);
    
    return;
}
```



 

 




